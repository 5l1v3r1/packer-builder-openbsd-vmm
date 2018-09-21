# packer-builder-openbsd-vmm
[Packer](https://packer.io/) builder plugin for OpenBSD's VMM

# Building

```
go build -o ~/.packer.d/plugins/packer-builder-openbsd-vmm
```

# Example template

```
{
  "builders": [
      {
          "type": "openbsd-vmm",
          "image_name": "some-image",
          "user_data": "",
          "ssh_username": "root"
      }
  ]
}
```

# Remarks
This is heavily based on https://github.com/m110/packer-builder-hcloud