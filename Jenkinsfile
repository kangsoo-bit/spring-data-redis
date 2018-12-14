pipeline {
  agent any
  stages {
    stage('Checkout/Subversion') {
      steps {
        svn(url: 'svn://122.199.232.37/svn/trunk/bitmiweb_boot', changelog: true, poll: true)
      }
    }
    stage('build') {
      steps {
        build 'bitmiweb_boot'
      }
    }
  }
}