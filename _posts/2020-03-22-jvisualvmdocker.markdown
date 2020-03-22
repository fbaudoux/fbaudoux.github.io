---
layout: post
title:  "Options to run a jvm for jvisualvm usage into docker"
date:   2020-03-22 22:24:34 +0200
categories: docker
---

```
-Dcom.sun.management.jmxremote
-Dcom.sun.management.jmxremote.port=9010
-Dcom.sun.management.jmxremote.local.only=false
-Dcom.sun.management.jmxremote.authenticate=false
-Dcom.sun.management.jmxremote.ssl=false
```

