 properties([pipelineTriggers([pollSCM('H/30 * * * *')])])node{
    stage("clone"){
        git "https://github.com/Taldah/Devops2702.git"
    }
    stage("execute"){
      sh  'git add .'
      sh  'git commit -am "add jenkins file to my remo-repo"'
      sh  'git checkout NewButton'
      sh  'git merge master'
      sh  'git checkout master'
      sh  'git merge NewButton'
      sh  'git pull'
      sh  'git push'
 }
}