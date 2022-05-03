```
torres.s503@WIN-9KQ3VLQ3B6R MINGW64 ~/Desktop/devops-with-docker/part1/1.7
$ docker build . -t web-server
[+] Building 0.1s (5/5) FINISHED
 => [internal] load build definition from Dockerfile                                                                                                                        0.0s
 => => transferring dockerfile: 96B                                                                                                                                         0.0s
 => [internal] load .dockerignore                                                                                                                                           0.0s
 => => transferring context: 2B                                                                                                                                             0.0s
 => [internal] load metadata for docker.io/devopsdockeruh/simple-web-service:alpine                                                                                         0.0s
 => [1/1] FROM docker.io/devopsdockeruh/simple-web-service:alpine                                                                                                           0.1s
 => exporting to image                                                                                                                                                      0.0s
 => => exporting layers                                                                                                                                                     0.0s
 => => writing image sha256:978fbf315695ef5a3ec2e77ee411c4dcd9aa9b867fbc7ea3d26962545fda0585                                                                                0.0s
 => => naming to docker.io/library/web-server                                                                                                                               0.0s

Use 'docker scan' to run Snyk tests against images to find vulnerabilities and learn how to fix them

torres.s503@WIN-9KQ3VLQ3B6R MINGW64 ~/Desktop/devops-with-docker/part1/1.7
$ docker run web-server
[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
 - using env:   export GIN_MODE=release
 - using code:  gin.SetMode(gin.ReleaseMode)

[GIN-debug] GET    /*path                    --> server.Start.func1 (3 handlers)
[GIN-debug] Listening and serving HTTP on :8080
```
