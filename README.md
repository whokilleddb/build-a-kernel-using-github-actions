# Did anyone try building the Linux kernel via GitHub Actions?

![](images/mihai_tweet.png)

It all started when I came across [this tweet](https://twitter.com/mihaimaruseac/status/1549779241759191040) by [@mihaimaruseac](https://github.com/mihaimaruseac) and decided to try it for myself (instead of studying for finals)

![](images/whokilleddb_tweet.png)

## How to trigger actions?
To trigger Github actions and start the compilation process, simply push to the `build` branch.

## Observations
- It takes approximately 2hrs 10mins to build the 5.18.14 kernel.
- We are compiling with the default configurations for Arch Linux (See [here](https://wiki.archlinux.org/title/Kernel/Traditional_compilation))
- Cache build is failing due to the system running out of memory (See [here](https://github.com/whokilleddb/build-a-kernel-using-github-actions/runs/7483738830?check_suite_focus=true))