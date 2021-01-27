<h1 align="center">
  <img src="https://github.com/Dreamacro/clash/raw/master/docs/logo.png" alt="Clash" width="200">
  <br>
  ClashX
  <br>
</h1>


A rule based proxy For Mac base on [Clash](https://github.com/Dreamacro/clash).



## Features

- HTTP/HTTPS and SOCKS protocol
- Surge like configuration
- GeoIP rule support
- Support Vmess/Shadowsocks/Socks5/Trojan
- Support for Netfilter TCP redirect

## Install

You can download from [Release](https://github.com/yichengchen/clashX/releases) page

**Download ClashX Pro With enhanced mode and Native Apple Silicon support  at [AppCenter](https://install.appcenter.ms/users/clashx/apps/clashx-pro/distribution_groups/public) for free permanently.**


## Build
- Make sure have python3 and golang installed in your computer.

- Install Golang
  ```
  brew install golang

  or download from https://golang.org
  ```

- Download deps
  ```
  bash install_dependency.sh
  ```

- Build and run.

## Config


The default configuration directory is `$HOME/.config/clash`

The default name of the configuration file is `config.yaml`. You can use your custom config name and switch config in menu `Config` section.


Checkout [Clash](https://github.com/Dreamacro/clash) or [SS-Rule-Snippet for Clash](https://github.com/Hackl0us/SS-Rule-Snippet/blob/master/LAZY_RULES/clash.yaml) or [lancellc's gitbook](https://lancellc.gitbook.io/clash/) for more detail.

## Advance Config

### Change the ports of ClashX

  Please modify the `config.yaml` file generated by ClashX, not the other config file you created or downloaded. The `General` section settings in your custom config file would be ignored.


### Change your status menu icon

  Place your icon file in the `~/.config/clash/menuImage.png`  then restart ClashX.

### Change default system ignore list.

- Download sample plist in the [Here](proxyIgnoreList.plist) and place in the

  ```
  ~/.config/clash/proxyIgnoreList.plist
  ```

- Edit the `proxyIgnoreList.plist` to set up your own proxy ignore list

### Use url scheme to import remote config.

- Using url scheme describe below

  ```
  clash://install-config?url=http%3A%2F%2Fexample.com&name=example
  ```


