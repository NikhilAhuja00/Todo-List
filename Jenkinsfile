node {
    def frontend
    def backend
    checkout scm

    stage('BUILD_STAGE') {
    
        frontend = docker.build("ahujanikhil30/frontend","./todo-list")
        backend = docker.build("ahujanikhil30/backend","./server_logic")

    }

    stage('PUSH_STAGE') {
        docker.withRegistry('https://registry.hub.dockr.com','docker-hub') {
            frontend.push()
            backend.push()
        }
    }
}