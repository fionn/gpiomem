On Arch Linux, `/dev/gpiomem` is restricted to `root`. This means ordinary users can't use GPIO pins.

Install with `install -m 644 -t /etc/systemd/system/ gpiomem.service`.
By enabling `gpiomem.service`, users in the `gpio` group will get automatic access.
