#DEPRECATION: Option 'glvnd' value 'true' is replaced by 'enabled'
OPTS+=" -D b_lto=true \
        -D build-tests=false \
        -D b_ndebug=true \
        -D platforms=x11,wayland \
        -D shader-cache=auto \
        -D glx=dri \
        -D gbm=enabled \
        -D egl=enabled \
        -D gles2=enabled \
        -D gles1=disabled \
        -D glvnd=enabled \
        -D valgrind=disabled \
        -D shared-glapi=enabled \
        -D libunwind=enabled \
        -D vulkan-drivers=auto \
        -D vulkan-layers=device-select,intel-nullhw,overlay,screenshot,vram-report-limit \
        -D video-codecs=all \
        -D gallium-drivers=auto \
        -D gallium-va=enabled \
        -D gallium-xa=enabled \
        -D gallium-nine=true \
        -D gallium-vdpau=enabled \
        -D gallium-extra-hud=true \
        -D gallium-opencl=disabled \
        -D gallium-va=enabled \
        -D microsoft-clc=disabled \
        -D intel-clc=enabled \
        -D install-intel-clc=true \
        -D llvm=enabled \
        -D osmesa=true"

default_meson_build &&

# indirect rendering
ln -sf /usr/lib/libGLX_mesa.so.0 /usr/lib/libGLX_indirect.so.0
