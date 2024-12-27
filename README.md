# MiniEAP-SYSU

在 [minieap](https://github.com/updateing/minieap) 的基础上为适配 SYSU 校园网环境进行的适配版本。

## 编译

> 如果要在 OpenWrt 上使用此项目，建议移步 [openwrt-minieap-sysu](https://github.com/Undefined443/openwrt-minieap-sysu)（minieap 主程序）和 [luci-app-minieap](https://github.com/kongfl888/luci-app-minieap)（minieap Web 管理插件）。它们是这个项目的 OpenWrt 适配版。

1. 下载你路由器型号的 Toolchain：

   [ImmortalWrt Firmware Selector](https://firmware-selector.immortalwrt.org/)

   [OpenWrt Firmware Selector](https://firmware-selector.openwrt.org/)

2. 克隆源码。
3. 修改 `config.mk`，将其中的 `CC` 修改为 Toolchain 中 GCC 编译器的路径。
4. 使用 `make` 编译。

## 运行

```sh
./minieap -u <username> -p <password> -n <nic>
```
