# openrex_uboot_v2017_10
mx6q/dl/s/spl openrex u-boot v2017.10 
 
# Download repository
    git clone https://github.com/R16-Rubus/rubus-uboot-v2017.03
    cd rubus-uboot-v2017.03
 
# Install cross compiler
    apt-get install gcc-arm-linux-gnueabihf
 
# Setup cross compiler
    export CROSS_COMPILE=arm-linux-gnueabihf-
    export ARCH=arm
 
# Build (imx6q)
    make distclean
    make r16qrubus_config
    make
    cp u-boot.imx /tftp/uboot-r16qrubus.imx
 
# Build (imx6dl)
    TODO
 
# Build (imx6s)
    TODO
