# Example of android sharing texture with linux by using  DMA-BUF

An example of how to share a GL/GLES texture in EGL context between android and linux  processes by using DMA-BUF.

Detailed explanation is in [this blog post](https://blaztinn.gitlab.io/post/dmabuf-texture-sharing/).

Prerequisites:

  - Linux OS (for dma-buf and [unix domain sockets](https://en.wikipedia.org/wiki/Unix_domain_socket))
  - EGL extensions:
    - [EGL_MESA_image_dma_buf_export](https://www.khronos.org/registry/EGL/extensions/MESA/EGL_MESA_image_dma_buf_export.txt)
    - [EGL_EXT_image_dma_buf_import](https://www.khronos.org/registry/EGL/extensions/EXT/EGL_EXT_image_dma_buf_import.txt)
  - GLES extensions:
    - [GL_OES_EGL_image_external](https://www.khronos.org/registry/OpenGL/extensions/OES/OES_EGL_image_external.txt)

Build:

``` bash
$ make
```

Run:

$ ./dmabufshare client
```
