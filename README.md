Test project to get externals working with libpd and Android.

2013/01/25
- Downloaded freeverb source.
- Downloaded latest NDK, android-ndk-r8d. Setup and tested, was able to get  a the sample hello-jni app working.
- Setup Android.mk file in project jni folder along with freeverb source code.
- Ran ndk-build from cygwin, completed sucessfully, creating libfreeverb_tilde.so files as can be seen in libs dir. 
- Ran app and first time... no reverb. Ran a second time with no changes and reverb magically worked. Uninstalled, reinstalled the app and again, no reverb. Re run, and reverb suddenly works fine.

Not sure what is causing this behaviour, would appreciate any help!

Been following this thread:

http://createdigitalnoise.com/discussion/1816/using-externals-with-libpd#Item_14

In hopes of a solution. 
