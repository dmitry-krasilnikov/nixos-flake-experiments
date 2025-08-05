# Run VM

```nu
nixos-rebuild build-vm --flake .#test
# expose port 22 from guest
$env.QEMU_NET_OPTS = "hostfwd=tcp::2221-:22"
./result/bin/run-nixos-vm
```

# Credits

- https://gist.github.com/FlakM/0535b8aa7efec56906c5ab5e32580adf
