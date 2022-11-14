pipeline
{
    agent any
    stages
    {
        stage("build")
        {
            agent
            {
                label 'ashu-vm-node-1'
            }
            steps
            {
                sh'echo "This is from another VM build"'
            }
        }
        stage("test")
        {
            agent
            {
                label 'ashu-VM-node-2'
            }
            steps
            {
                sh'echo "This is from another VM test"'
            }
        }
        stage("deploy")
        {
            agent
            {
                label 'ashu-node-1'
            }
            steps
            {
                sh'echo "This is from another VM deploy"'
            }
        }
    }
}
