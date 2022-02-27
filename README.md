# DO NOT USE

The thing you're looking for is here: https://github.com/yt-dlp/FFmpeg-Builds

Below for original README.

# FFmpeg Static Auto-Builds


This repository provides static Windows (x86 and x86_64) and Linux (x86_64) Builds of [ffmpeg master](https://github.com/FFmpeg/FFmpeg) and [latest release branch](https://github.com/FFmpeg/FFmpeg/tree/release/4.4) **with some patches necesssary for smooth integration with [yt-dlp](https://github.com/yt-dlp/yt-dlp)**

**Note**: The builds provided are only meant to be used with yt-dlp and any unrelated issues/patches will be rejected


## Downloads

[![Linux x64 GPL master](https://img.shields.io/badge/-Linux_x64-red.svg?style=for-the-badge&logo=linux)](https://github.com/yt-dlp/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-linux64-gpl.tar.xz "Linux x64 GPL master")
[![Windows x64 GPL master](https://img.shields.io/badge/-Windows_x64-blue.svg?style=for-the-badge&logo=windows)](https://github.com/yt-dlp/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-gpl.zip "Windows x64 GPL master")
[![Windows x86 GPL master](https://img.shields.io/badge/-Windows_x86-9cf.svg?style=for-the-badge&logo=windows)](https://github.com/yt-dlp/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win32-gpl.zip "Windows x86 GPL master")
[![Other variants](https://img.shields.io/badge/-Other-grey.svg?style=for-the-badge)](https://github.com/yt-dlp/FFmpeg-Builds/wiki/Latest "All variants")
[![Other versions](https://img.shields.io/badge/-Old_Versions-lightgrey.svg?style=for-the-badge)](https://github.com/yt-dlp/FFmpeg-Builds/releases "All releases")

---




## Patches Welcome
Known issues for which patches are welcome

<!--
*Nothing at the moment*
-->

#### 1. MacOS/ARM Builds

There are currently no MacOS/ARM builds. If you know how to add them to the workflow, make a PR



## Patches Applied
These patches have been applied to the builds

#### 1. [Long path support for Windows](https://ffmpeg.org/pipermail/ffmpeg-devel/2022-February/292947.html)
by [@nihil-admirari](https://github.com/nihil-admirari)
Fixes [yt-dlp#1995](https://github.com/yt-dlp/yt-dlp/issues/1995), [yt-dlp#1273](https://github.com/yt-dlp/yt-dlp/issues/1273), [FFmpeg#8885](https://trac.ffmpeg.org/ticket/8885)


## Historical Patches
Patches that were used in the past but are no longer needed

#### 1. [Fix AAC HLS streams being truncated mid stream](https://patchwork.ffmpeg.org/project/ffmpeg/patch/20210927213133.28258-1-jeebjp@gmail.com)
by [@shirt](https://github.com/shirt-dev) and [@jeeb](https://github.com/jeeb), merged in [c205778](https://github.com/FFmpeg/FFmpeg/commit/c20577806f0a161c6867e72f884d020a253de10a))  
Fixes [yt-dlp#618](https://github.com/yt-dlp/yt-dlp/issues/618), [yt-dlp#998](https://github.com/yt-dlp/yt-dlp/issues/998), [yt-dlp#1039](https://github.com/yt-dlp/yt-dlp/issues/1039), [FFmpeg#9433](https://trac.ffmpeg.org/ticket/9433)

#### 2. [Fix for YouTube's VP9 encodes with non-monotonous DTS](https://ffmpeg.org/pipermail/ffmpeg-devel/2021-May/280189.html)
by [@danny-wu](https://github.com/danny-wu), merged in [68595b4](https://github.com/FFmpeg/FFmpeg/commit/68595b46cb374658432fff998e82e5ff434557ac)  
Fixes [yt-dlp#871](https://github.com/yt-dlp/yt-dlp/issues/871), [youtube-dl#28042](https://github.com/ytdl-org/youtube-dl/issues/28042), [FFmpeg#9086](https://trac.ffmpeg.org/ticket/9086)



## Credits

* [@BtbN](https://github.com/BtbN) for the [original workflow](https://github.com/BtbN/FFmpeg-Builds)
* [@nihil-admirari](https://github.com/nihil-admirari) for creating and maintaining this repo

---

PS: The commits are unsigned because of the periodic [automatic rebase](https://github.com/yt-dlp/FFmpeg-Builds/actions/workflows/rebase-on-upstream.yml)
