# skopeo-binary

[![Build](https://github.com/lework/skopeo-binary/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/lework/skopeo-binary/actions/workflows/build.yml)

Generate [skopeo](https://github.com/containers/skopeo) binaries.

## Useage

The [release](https://github.com/lework/skopeo-binary/releases) version of the project is the same as the [skopeo](https://github.com/containers/skopeo/releases) release version, which can be viewed directly on the [ release](https://github.com/lework/skopeo-binary/releases) page directly.

```bash
version=v1.6.2
arch=amd64
[ -f /usr/bin/skopeo ] && mv /usr/bin/skopeo{,_src}
wget https://github.com/lework/skopeo-binary/releases/download/${version}/skopeo-linux-${arch} -O /usr/bin/skopeo
chmod +x /usr/bin/skopeo
```