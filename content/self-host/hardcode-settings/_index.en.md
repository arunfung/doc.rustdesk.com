---
title: Hardcoding Custom Settings 
weight: 49
---

## Custom Server
{{% notice note %}}
To hardcode custom server settings into your executables you must [build](/docs/en/dev/build/) the client yourself on your machine or [with GitHub Actions](/docs/en/dev/build/all/).
{{% /notice %}}
{{% notice note %}}
**If you set either of these values without setting the other, your executable will not work!**
{{% /notice %}}

You can set the following environment variables on your OS and rustdesk will use those variables when compiling your client rather than the default rustdesk.com servers. 

If you do not know how to set an environment variable on your system you should be able to find documentation for your OS online that will explain this.

#### RENDEZVOUS_SERVER
This variable should be set to your server URL.

This should be a string such as
```
rustdesk.my-domain.com
```

#### RS_PUB_KEY
This variable will be your public key, more information on the key is available [here](/docs/en/self-host/install/#key).

This should be a string such as
```
OeVuKk5nlHiXp+APNn0Y3pC1Iwpwn44JGqrQCsWqmBw=
```
