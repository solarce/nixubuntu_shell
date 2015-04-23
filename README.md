nixubuntu_shell
==============

A 14.04 based Docker container with the latest stable Nix and some handy
Nix tools installed.

It's designed to let you work on code with Nix available, by mounting
your $HOME into the container.

Usage
====

```
7888 ◯ : docker run -it -u ubuntu -v $HOME:/home/ubuntu
solarce/nixubuntu-shell
⏎
Unable to find image 'solarce/nixubuntu-shell:latest' locally
Pulling repository solarce/nixubuntu-shell
261ceffebb69: Download complete
706766fe1019: Download complete
a62a42e77c9c: Download complete
2c014f14d3d9: Download complete
b7cf8f0d9e82: Download complete
cc3a10135b0d: Download complete
ebfe4cfc0eab: Download complete
0839b627de77: Download complete
5319a779e5ab: Download complete
d71f46560955: Download complete
31582687029b: Download complete
7573cbb79f41: Download complete
9b83ab9dabe4: Download complete
fe6816634e4f: Download complete
96d03a7a3f8a: Download complete
cea160f5c5a3: Download complete
e3f6bbe1634d: Download complete
7a05f4414034: Download complete
Status: Downloaded newer image for solarce/nixubuntu-shell:latest
[ubuntu@4e1f9fcbc0cd ~]$ zsh

4e1f9fcbc0cd 福 ~
7892 ◯ : ls
code  

4e1f9fcbc0cd 福 ~
7893 ◯ : cd code/pipeline/

4e1f9fcbc0cd 福 ~/code/pipeline ➤ 315f60a|pipeline-docs✓
7894 ± : git st
[50d1h33m]
On branch pipeline-docs
Your branch is up-to-date with 'origin/pipeline-docs'.

nothing to commit, working directory clean

4e1f9fcbc0cd 福 ~/code/pipeline ➤ 315f60a|pipeline-docs✓
7895 ± :
```
