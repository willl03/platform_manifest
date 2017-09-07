##Initialize the source## repo init -u https://github.com/willl03/platform_manifest.git -b W03-8.0

##Sync the source## repo sync -jx -f (x being however many cpu jobs)

##Setup build environment## . build/envsetup.sh

##Get the right device to build## lunch aosp_angler-user

##Build it## make otapackage -jx (x being however many cpu jobs)