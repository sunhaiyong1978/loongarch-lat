FROM ghcr.io/yongbaoos/target_base:glibc_2.43
ARG TARGETARCH

ARG DEPENDENCIES="         \
        gcc                \
        g++                \
        make               \
        git                \
        ninja-build        \
        meson              \
        openssl-devel      \
        glib2-devel        \
        tar"

RUN \
    wget -c https://mirrors.wsyu.edu.cn/fedora/linux/Yongbao/tar_install/gcc_16.1.0/loongarch64-Yongbao-sysroot.devel.tar.xz \
    && tar -xpf loongarch64-Yongbao-sysroot.devel.tar.xz -C / \
    && rm -f loongarch64-Yongbao-sysroot.devel.tar.xz

RUN git config --global --add safe.directory /io
