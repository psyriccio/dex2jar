# dex2jar
Tools to work with android .dex and java .class files

###Components:

* dex-reader is designed to read the Dalvik Executable (.dex/.odex) format. It has a light weight API similar with ASM. An example here
* dex-translator is designed to do the convert job. It reads the dex instruction to dex-ir format, after some optimize, convert to ASM format.
* dex-ir used by dex-translator, is designed to represent the dex instruction
* dex-tools tools to work with .class files. here are examples:
* Modify a apk
* DeObfuscate a jar
* d2j-smali [To be published] disassemble dex to smali files and assemble dex from smali files. different implementation to smali/baksmali, same syntax, but we support escape in type desc "Lcom/dex2jar\t\u1234;"
* dex-writer [To be published] write dex same way as dex-reader.

###Looking for help
Please send email to dex2jar@googlegroups.com or post at dex2jar-google-group

###News
* Oct 25, 2012, dex2jar-0.0.9.11 add support to strict type analyze. It's ok to dex-jar-dex now.
* Oct 21, 2012, dex2jar-0.0.9.10 add support to generate the access flag for inner class.
* Jan 2, 2012, dex2jar-0.0.9.5 add support to work with .class files.
* Dec 25, 2011, dex2jar-0.0.9.4 add support to translate ICS dex file and read odex file
* Nov 10, 2011, dex2jar-0.0.9.3 can translate apks in android-2.3.3 emulator(/system/app/x.apk)
* Nov 03, 2011, add Jenkins: https://dex2jar.ci.cloudbees.com/ and maven repo: http://repository-dex2jar.forge.cloudbees.com/release/
* Nov 02, 2011, Code generated by dex2jar-0.0.9.2 about commons-collections-3.2.1 can pass all junit test.
