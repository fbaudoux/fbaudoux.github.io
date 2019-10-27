---
layout: post
title:  "Pushing docker image to nexus OSS"
date:   2019-10-19 22:24:34 +0200
categories: linux ssh
---
I have a local image if my software __MyTool__ created from a dockerfile.  
I want to push it into my nexus repository as the version 1.0 of MyTool.  
Let's say my nexus is available on port 7777.  

I start by getting the image reference on my local system:  
```
 docker images
```

then I tag my image:  

```
 docker tag b3b8a2229953 @nexusIP:7777/mytool:1.0
```

and I push it to nexus:  
```
 docker push @nexusIP:7777/mytool:1.0
```
