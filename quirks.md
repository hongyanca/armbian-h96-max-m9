**Armbian Config** (`armbian-config`) is a lightweight, **interactive and scriptable** configuration utility that automates the common tasks of setting up and maintaining an Armbian system. It ships **preinstalled** on every Armbian image and is especially handy on single-board computers (SBCs)

```
sudo armbian-config
```

---

`uv`

Running `uv` on CPU 0 avoided the crash:

```
taskset -c 0 uv <your command>
```

---

Turn off SWAP

Set `SWAP=false` in `/etc/default/armbian-zram-config`