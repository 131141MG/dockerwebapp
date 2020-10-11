node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("mg102020/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
