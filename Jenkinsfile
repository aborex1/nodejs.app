node {
    checkout scm

    docker.withRegistry('https://github.com/aborex1/nodejs.app.git', 'github101') {

        def customImage = docker.build("myapp/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
