stage "unit test"
sh "pwd"

node {
   echo "node stage is started"
   git "https://github.com/forpix/Alto-1.git"
   sh "echo unit test app"
   echo "========================================"
}

stage "test on supported OSes"

parallel (
  windows: { node {
    sh "echo building on windows now"

 }},
  mac: { node {
    sh "echo building on mac now"
}})
