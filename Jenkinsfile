node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("admin0506/SecurityTestingRepo")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}