properties([pipelineTriggers([pollSCM('H/30 * * * *')])])node{
    stage("clone"){
        git "https://github.com/Taldah/Devops2702.git"
    }
    stage("execute"){
       git 'add .'
       git 'commit -am "add jenkins file to my remo-repo"'
       git 'checkout NewButton'
       git 'merge master'
       git 'checkout master'
       git 'merge NewButton'
       git 'pull'
       git 'push'
 }
}
