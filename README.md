## Inspired by [ipinfw.tw](https://github.com/PeterDaveHello/ipinfo.tw)

## Build

If you want to build your own image, instead of directly pull the pre-built one, clone this repository, and run docker build command, with build-arg MAXMIND_LICENSE_KEY, you need to provide your own MaxMind license key from https://www.maxmind.com/en/account, it's free.

```bash
git clone --depth 1 https://github.com/killbus/nginx-ipfilter
cd nginx-ipfilter
docker build --build-arg MAXMIND_LICENSE_KEY="$MY_MAXMIND_KEY" -t ipfilter:custom-build .
```