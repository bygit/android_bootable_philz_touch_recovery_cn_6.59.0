#### Building

Clone philz recovery to bootable/recovery-philz folder

    git clone https://github.com/Mr-zeng/android_bootable_philz_touch_recovery_cn_6.59.0 -b cm-11.0

Now build with RECOVERY_VARIANT flag set to philz:

    . build/envsetup.sh && lunch && mka -j3 recoveryimage RECOVERY_VARIANT=philz

or

    export RECOVERY_VARIANT=philz
    . build/envsetup.sh && lunch && mka -j3 recoveryimage

or

    add to device BoardConfig.mk:
        RECOVERY_VARIANT := philz
    and run:
        build/envsetup.sh && lunch && mka -j3 recoveryimage
