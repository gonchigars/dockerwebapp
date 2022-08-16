node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockhubid') {

        def customImage = docker.build("topkuber/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
