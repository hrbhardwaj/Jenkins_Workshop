# Jenkins_Workshop

## Deployment 
In this Deployment Jenkinsfile:

* We define environment variables for Kubernetes configuration (KUBECONFIG), Docker registry credentials (DOCKER_REGISTRY_CREDENTIALS), your application's name (APP_NAME), 
   and the image tag.
* There are stages for checking out your source code, building a Docker image, pushing it to a container registry, deploying it to Kubernetes, and cleaning up any resources.
* In the "Deploy to Kubernetes" stage, we use kubectl to apply the Kubernetes manifests for your application, and we also wait for the deployment to complete.
* In the post section, we define actions to take based on the success or failure of the pipeline.
