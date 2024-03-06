pipeline {
  agent {
    docker {
image 'node: 14'
}
}
stages {
stage( 'Clone repository') {
steps {
git branch: 'main',
url: 'https://github.com/<user>/<repo>.git'
Stage('Install dependencies ') (
steps 1
sh 'npm install'
Stage(' Build application') (
steps {
sh 'npm run build'
｝
stage ('Test application) (
steps {
sh 'npm test'
}
Stage (" Push Docker image')s
steps t
sh 'docker build -t ‹user>/<image>: $BUILD_NUMBER .' sh docker push ‹user>/<image>: $BUILD_NUMBER'
}
}
}
}
