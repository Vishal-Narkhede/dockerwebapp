node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("vnark01/nodeApplication")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
