Package: gamenetworkingsockets:x64-windows@1.4.1#1

**Host Environment**

- Host: x64-windows
- Compiler: MSVC 19.38.33135.0
-    vcpkg-tool version: 2025-07-21-d4b65a2b83ae6c3526acd1c6f3b51aff2a884533
    vcpkg-scripts version: 3bdaa9b420 2025-07-27 (31 hours ago)

**To Reproduce**

`vcpkg install `

**Failure logs**

```
Downloading https://github.com/ValveSoftware/GameNetworkingSockets/archive/505c697d0abef5da2ff3be35aa4ea3687597c3e9.tar.gz -> ValveSoftware-GameNetworkingSockets-505c697d0abef5da2ff3be35aa4ea3687597c3e9.tar.gz
error: https://github.com/ValveSoftware/GameNetworkingSockets/archive/505c697d0abef5da2ff3be35aa4ea3687597c3e9.tar.gz: failed: status code 503
note: If you are using a proxy, please ensure your proxy settings are correct.
Possible causes are:
1. You are actually using an HTTP proxy, but setting HTTPS_PROXY variable to `https//address:port`.
This is not correct, because `https://` prefix claims the proxy is an HTTPS proxy, while your proxy (v2ray, shadowsocksr, etc...) is an HTTP proxy.
Try setting `http://address:port` to both HTTP_PROXY and HTTPS_PROXY instead.
2. If you are using Windows, vcpkg will automatically use your Windows IE Proxy Settings set by your proxy software. See: https://github.com/microsoft/vcpkg-tool/pull/77
The value set by your proxy might be wrong, or have same `https://` prefix issue.
3. Your proxy's remote server is our of service.
If you believe this is not a temporary download server failure and vcpkg needs to be changed to download this file from a different location, please submit an issue to https://github.com/Microsoft/vcpkg/issues
CMake Error at scripts/cmake/vcpkg_download_distfile.cmake:136 (message):
  Download failed, halting portfile.
Call Stack (most recent call first):
  scripts/cmake/vcpkg_from_github.cmake:120 (vcpkg_download_distfile)
  C:/Users/sidsh/AppData/Local/vcpkg/registries/git-trees/75eaecf85e526c7de535e77ac6da7025c8e4020f/portfile.cmake:3 (vcpkg_from_github)
  scripts/ports.cmake:206 (include)



```

**Additional context**

<details><summary>vcpkg.json</summary>

```
{
  "dependencies": [
    "gamenetworkingsockets"
  ]
}

```
</details>
