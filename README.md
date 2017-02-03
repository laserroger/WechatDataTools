# WechatDataTools
Performs some analysis with WeChat chat data
------
## Features

- Statistics for all chats: see who chat with you most in total, or over a period of time.

- Statistics for one person: see the change of frequency of your conversations.

- Export all chat history to a CSV file. (Other tools with this functionality for iOS I have found so far ask for money)

- If you can understand the code, it is easy write other functions to discover more from your chat history, for example, semantics analysis, etc. I don't have that much extra time to implement more.

## Requirements

Mathematica 10.3 or above. Some functions used are newly introduced, like `Nothing` in 10.3, `UpTo` and `DateHistogram` in 10.2. You can use lower version if you can make minor changes to get it to work.

**This program is written for iOS, it is not tested on Android since I do not own one.**
**There are much easier ways to extract chat history on Android, even Windows Wechat client has such a feature.**

The notebook includes all instructions after obtaining the app documents of Wechat. Here is a guide on obtaining those files.
Starting from iOS 8.3, applications with file-sharing not enabled will be blocked from third party access without jailbreak, which made the process painful, but there are still methods.

1. If your iOS device running wechat is jailbroken, you can either (use openssh) or (install AFC2 and access with third party tools), the documents of wechat is located in `/var/mobile/Containers/Data/Application/<app id>/Documents`

2. If your phone running wechat is not jailbroken, but one of your other devices is, you can perform a chat history transfer(in wechat app), and then follow method 1.

3. If none of your devices are jailbroken, perform a complete backup. Then use third party tools that can read and extract from a backup to extract the files.

I know the description above is missing a lot of details, but I believe you can do it after some google search. It is Apple that made this process painful. Good luck.

**Last Note: If you find that the database structure for chat history is changed, please raise an issue and I will try to update it.**
