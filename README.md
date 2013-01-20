maserati_jb-mr1_manifest
========================

#THIS IS NOT YET BUILDABLE. CURRENT PROGRESS 30%
#Check back soon for updates

Android 4.2.1_r1 Manifest for Droid 4
Based off of the wonderful work done by STS_Dev_team, DHacker29, and Hashcode. All credits for their work go to them appropriately. 
This build is a google AOSP attempt based on unmodded google source code. Device and Vendor files were imported from STS and were
modified to work with this branch of the AOSP code.

To initialize a build environment perform the following commands:

mkdir 4.2.1_r1

cd 4.2.1_r1

repo init -u https://android.googlesource.com/platform/manifest -b android-4.2.1_r1

curl -L -o .repo/local_manifest.xml -O -L https://raw.github.com/greek35t/maserati_jb-mr1_manifest/master/local_manifest.xml

Then sync up with : repo sync

build code with: make -j4

Currently our releaseutils are not built yet so you will have to package the output into a zip for flashing.

You will need to also flash the google apps 12122012 which can be found at http://goo.im/gapps/gapps-jb-20121212-signed.zip

Enjoy! Please send bug reports to greek35t@gmail.com
