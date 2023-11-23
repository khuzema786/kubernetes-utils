# Counter Application to demo kubernetes
Its a simple counter app which logs and increments the count from a file. Repository includes Dockerfile and respective kubernetes manifest.

The image is already pushed at docker.io/khuzema786/counter. You can use that or build and run the app yourself using the following commands.

`docker build -t counter . && docker tag counter khuzema786/counter && docker push khuzema786/counter`

Deploy on Kubernetes
You can deploy on kubernetes using the manifests present in kubernetes folder. I have used Persistent Volumes so that when scaling replicas of Deployments or Statefulsets, you can easily see the difference.