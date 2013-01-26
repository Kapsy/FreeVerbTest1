Test project to get externals working with libpd and Android.

2013/01/25
- Downloaded freeverb source.
- Downloaded latest NDK, android-ndk-r8d. Setup and tested, was able to get  a the sample hello-jni app working.
- Setup Android.mk file in project jni folder along with freeverb source code.
- Ran ndk-build from cygwin, completed sucessfully, creating libfreeverb_tilde.so files as can be seen in libs dir. 
- Ran app and first time... no reverb. Ran a second time with no changes and reverb magically worked. Uninstalled, reinstalled the app and again, no reverb. Re run, and reverb suddenly works fine.

See the following thread for details:

http://createdigitalnoise.com/discussion/1816/using-externals-with-libpd#Item_14

2013/01/26

Thanks to Nitrooo from the above forum solution was simple: initAudio() must be called before PdBase.openPatch(patchfile).

Leaving this git here if anyone doesn't know where to start with externals :).

