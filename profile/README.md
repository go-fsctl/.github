<p align="center"><img src="https://raw.githubusercontent.com/go-fsctl/brand/main/social/go-fsctl.png" alt="go-fsctl" width="640"></p>

<h1 align="center">go-fsctl</h1>
<p align="center">Pure-Go control of Linux storage &amp; filesystem kernel subsystems — driven straight through the <code>ioctl</code> interfaces, with <strong>no cgo</strong> and <strong>no shelling out</strong> to CLIs.</p>
<p align="center">
  <img src="https://img.shields.io/badge/Go-1.26-00ADD8?style=flat-square&logo=go&logoColor=white">
  <img src="https://img.shields.io/badge/license-BSD--3--Clause-0A6E96?style=flat-square">
  <a href="https://github.com/go-volumes"><img src="https://img.shields.io/badge/pairs%20with-go--volumes-0079A8?style=flat-square"></a>
  <a href="https://github.com/go-filesystems"><img src="https://img.shields.io/badge/pairs%20with-go--filesystems-0079A8?style=flat-square"></a>
</p>

## Repositories

| Repo | What it is |
| --- | --- |
| [`dm`](https://github.com/go-fsctl/dm) | Linux **device-mapper** control via the `DM_*` ioctls — no `dmsetup` |
| [`btrfs`](https://github.com/go-fsctl/btrfs) | **btrfs** kernel control via the `BTRFS_IOC_*` ioctls — no CLI |
| [`zfs`](https://github.com/go-fsctl/zfs) | **libzfs_core**-style ZFS kernel operations via `/dev/zfs` ioctls — no CLI |
| [`loop`](https://github.com/go-fsctl/loop) | Linux **loop-device** control via `/dev/loop-control` + `LOOP_*` ioctls — no `losetup` |
| [`cowclone`](https://github.com/go-fsctl/cowclone) | **Copy-on-write file cloning** — APFS `clonefile(2)` + Linux `FICLONE` reflink, with a transparent byte-copy fallback |

Every repo is pure Go (`CGO_ENABLED=0`) and BSD-3-Clause.
