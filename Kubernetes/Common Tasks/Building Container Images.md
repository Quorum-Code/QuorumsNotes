#kubernetes #images
# How to Build a Container Image
1. Compile your application
2. Choose a base container image
	1. Using Docker
	2. Create a Dockerfile, [example in video](https://kubebyexample.com/learning-paths/kubernetes-fundamentals/building-images)
	3. Run `docker build -t <tag:vx.x> .`
	4. Push to Docker registry, `docker push <tag:vx.x>`