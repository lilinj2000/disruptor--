pipeline {
  agent any
  stages {
    stage('install') {
      steps {
        sh '''kernel=`uname -sr | sed --e=\'s/ /\\//\'`

home_3rd=$JENKINS_HOME/3rd/${kernel}

home_disruptor=${home_3rd}/disruptor

mkdir -p ${home_disruptor}/include

cp -avr disruptor ${home_disruptor}/include


'''
      }
    }
  }
}