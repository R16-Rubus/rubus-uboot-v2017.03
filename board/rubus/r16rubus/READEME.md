 rubus_uboot_v2015_10
mx6q/dl/s/spl r16rubus u-boot v2015.10 
 
# Download repository
    git https://github.com/R16-Rubus/rubus-uboot-v2017.03
    cd rubus-uboot-v2017.3
 
# Install cross compiler
    apt-get install gcc-arm-linux-gnueabihf
 
# Setup cross compiler
    export CROSS_COMPILE=arm-linux-gnueabihf-
    export ARCH=arm
 
# Build (imx6q)
    make distclean
    make r16rubus_config
    make
    cp u-boot.imx /tftp/uboot-r16rubus.imx
 
# Build (imx6dl)
    TODO
 
# Build (imx6s)
    TODO