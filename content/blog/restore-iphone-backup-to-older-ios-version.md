+++
author = "Anurag Upadhaya"
title = "How to restore iOS/iPhone backup to an older iOS version"
date = "2024-07-29"
description = "How to redirect www to domain apex on Cloudflare pages"
tags = [
    "iOS",
    "TIL",
]
+++

### TLDR - If you've insatlled iOS 18 public beta, without creating a full iOS 17 backup on your computer, you can restore an iOS 18 backup to iOS 17 by modifying the `Product Version` in `Info.plist` file present in the local backup.

I recently gave it to the curiostiy and went ahead with installing iOS 18 beta on my iPhone (all thanks to the Apple beta software program I had signed up for years ago), without being careful enough to create a iOS 17 archive backup in case I need to revert back.

After trying out the beta, I began searching for ways to revert back to the regular iOS 17 version. After reading through a couple of tutorials <sup>[1](https://www.macrumors.com/how-to/downgrade-from-ios-18-beta-to-ios-17/)</sup> <sup>[2](https://www.cnet.com/tech/mobile/ios-18-beta-second-thoughts-the-no-stress-way-to-go-back-to-ios-17/)</sup> , I had 2 big revelations:

* I did not bother creating a local archive backup on iOS 17

* I cannot use an iCloud backup to restore since it's overwritten by iOS 18

After digging through a couple of Reddit threads, I came across this [article](https://reincubate.com/support/how-to/restore-ios-backup-to-older-ios-device/) through which I was able to create an iOS 18 backup and then restore iPhone back to iOS 17 alongwith all the data from the same backup.

<small>Sources:</small>

1) https://www.macrumors.com/how-to/downgrade-from-ios-18-beta-to-ios-17/

2) https://www.cnet.com/tech/mobile/ios-18-beta-second-thoughts-the-no-stress-way-to-go-back-to-ios-17/

3) https://reincubate.com/support/how-to/restore-ios-backup-to-older-ios-device/