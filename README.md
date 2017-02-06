ATHENE-CAF
===========

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository using the AOSP-CAF trees, use a command like this:

    repo init -u https://github.com/athene-caf/platform_manifest.git -b n-mr1

Then to sync up:

    repo sync -c -f -j8 --force-sync --no-clone-bundle --no-tags

Building the source
---------------

    $ . build/envsetup.sh
    $ lunch aosp_athene-userdebug
    $ make -jX otapackage

where X is the number of jobs you would like to allot to the build system.

Other Devices
---------------

    We follow LA.BR.1.3.X branches from CAF. So if your device is based on the same ,you can go ahead and build ROM using this sources.
