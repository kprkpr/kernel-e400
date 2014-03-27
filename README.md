Requisitos
Entorno de desarrollo basico (Google)
Toolchains:  git clone https://github.com/DooMLoRD/android_prebuilt_toolchains.git

Instrucciones

export ARCH=arm

export SUBARCH=arm

make mrproper

make icsconfige0_defconfig

make V=0 -j2 CROSS_COMPILE=/home/---/android_prebuilt_toolchains/arm-eabi-4.4.3/bin/arm-eabi- zImage

--
Y en /arch/arm/boot estará la zImage
Puedes cambiar -j2 por otro numero mas alto para hacer más procesos a la vez,aunque lo más seguro parece ser -j2
