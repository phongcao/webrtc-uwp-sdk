# Instructions

From your terminal, recursively clone this repo to obtain all the source code needed to build WebRTC for UWP:
git clone --recursive https://github.com/webrtc-uwp/webrtc-uwp-sdk.git

This repository will yield the WebRtc SDK and dependency libraries.

Directory structure:

- webrtc-uwp-sdk\bin          	contains scripts for preparing an environment for the Windows
- webrtc-uwp-sdk\common         contains samples applications (ChatterBox and PeerCC)
- webrtc-uwp-sdk\webrtc    		contains WebRtc code
- webrtc-uwp-sdk\docs			contains documentation


Prerequisites:
- Visual Studio 2017 (latest tested version tested 15.6)
- Windows SDK 14393 (available from archive page https://developer.microsoft.com/en-us/windows/downloads/sdk-archive)
- The minimum required Windows version to deploy apps is 1607 / Build 10.0.14393 / Anniversary Update

## Windows Build

1. Run prepare script, from your terminal:
<br />
<pre>
<code>
cd webrtc-uwp-sdk
bin\prepare.bat
</code>
</pre>
<br />
This script will prepare environment but it won't build webrtc projects. In this case webrtc project will be built from Visual Studio once you try to build Org.WebRtc.

2. From VS2017, load webrtc\windows\solutions\WebRtc.sln for WebRtc development.

3. Now you can build UWP libraries for WebRtc and deploy sample app PeerCC.
