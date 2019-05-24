properties([gitLabConnection(''), parameters([choice(choices: 'master\nfeature-1\nfeature-2', description: 'select the branch to build', name: 'branch')])])

node {
    stage ('checkout scm') {
    echo "pulling chnages from the branch ${params.branch}"
    git url: 'https://github.com/linuxacademy/cicd-pipeline-train-schedule-cd', branch: "${params.branch}"
    }
}
