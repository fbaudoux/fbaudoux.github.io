---
layout: post
title:  "Enter into docker image to debug"
date:   2019-11-14 22:24:34 +0200
categories: docker
---
I have a local image of my software __MyTool__ created from a dockerfile.
When I try to run it, it fails and stop the container with no usefull message 

I start by getting the image reference on my local system:  
```
 docker run -it --entrypoint "/bin/sh" mytool:1.0
```

This command run a new container and override the entry point with "bin/sh"
I'm now able to navigate into my container. I can launch manually the entry point and see what happen
