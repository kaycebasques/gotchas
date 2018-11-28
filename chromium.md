# chromium

## [SSL: CERTIFICATE_VERIFY_FAILED]

### Repro

    gclient sync
    
### Error message

    INFO: Downloading package archive: binutils_arm_x86_64_apple_darwin.tgz (1/6) package_version: Could not download URL (https://storage.googleapis.com/nativeclient-once/object/binutils_arm_x86_64_apple_darwin_b33eac0121acfb07112b84a130824382abab91e2.tgz): <urlopen error [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed (_ssl.c:726)>
    Error: Command '/Library/Frameworks/Python.framework/Versions/2.7/Resources/Python.app/Contents/MacOS/Python src/build/download_nacl_toolchains.py --mode nacl_core_sdk sync --extract' returned non-zero exit status 1 in /Users/kayce/Repositories/chromium
    
### Solution

    /Applications/Python\ 2.7/Install\ Certificates.command
    
[Source](https://stackoverflow.com/questions/27835619/urllib-and-ssl-certificate-verify-failed-error#comment72358900_42334357)
