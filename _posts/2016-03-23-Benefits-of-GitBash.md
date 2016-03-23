---
layout: post
title: Benefits of GitBash
---

Before completing the tutorials on introduction to using the command line and data mining, I had been hesitant to use GitBash as my primary command line. At first, I was using PowerShell until the Internet Archive and WGET tutorials would not work with PowerShell, particularly at the first command of the Internet Archive tutorial "python -m pip install".

From there I began using the Command Prompt for Windows which worked fairly well but required re-learning some commands such as LS which is DIR in the Command Prompt. This was frustrating but I figured I could make do if it meant having a working command line. 

During the second lesson on API after I had created the metadata for my item, I received an error code `403 Write access denied`. This was extremely frustrating because I was excited to be able to try out all of the different types of items I could create with Zotero. At that time Shawn recommended to me that install GitBash and try to create a new Zotero item there. I was still unconvinced but installed it but only half-heartily retried the lesson using GitBash where I still did not receive the results the tutorial was looking for.

![create new Zotero item] (creating-new-item.png)

The introduction to Bash Command Line tutorial was doubly beneficial for me because it forced me to familiarize myself with GitBash. With a new understanding of GitBash, it also motivated me to go back and attempt to resolve my earlier issues. I realized quickly that commands I was using in the Command Prompt were going to be different in GitBash. Some searching online at Stackoverflow (http://stackoverflow.com/questions/32454589/git-2-5-1s-bash-console-doesnt-open-python-interpreter) quickly revealed that typing `python` into GitBash would not bring up the interpretor, but that `python -i` was required instead. Unfortunately the `403 Write acces denied` error did not fix itself in GitBash when I re-ran the script in GitBash.

![creating new item in GitBash] (create-new-item-git-bash.png)

Despite GitBash being a better option than Command Prompt, some of the instructions in the intro tutorial were still inconsistent with GitBash. Milligan writes that in Windows, help pwd will bring up the manual for the command. However, above he is discussing the manual for `ls` rather than `pwd` and gives no instructions for bringing up the ls manual in Windows. It is also not clear if by Windows he means using GitBash in Windows to make it more equivalent to OS X/Linux.

![command options] (help-ls.png)

Using GitBash in Windows, `help pwd` will bring up the manual for `pwd` but `help ls` does not bring up the manual for the ls command. Instead, GitBash requires `ls --help`. This is certainly not evident in the tutorial, which I will be noting on hypothesis.

Overall, GitBash required some re-working to follow along in the tutorial but is certainly better than PowerShell or Command Prompt. As we saw in the introduction tutorial, GitBash is not a direct equivalent to OS X/Linux and should not be treated as such. 
