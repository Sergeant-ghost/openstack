### This repository aims to make the OpenStack installation process more accessible, especially for those new to the platform. By following the provided instructions, users can quickly deploy an OpenStack cloud environment for development and testing purposes.

---

DevStack should be run as a non-root user with `sudo` enabled. Standard logins to cloud images such as “ubuntu” or “cloud-user” are usually fine.

If you are not using a cloud image, you can create a separate stack user:

```bash
sudo useradd -s /bin/bash -d /opt/stack -m stack
```

Ensure the home directory for the stack user has executable permissions for all:

```bash
sudo chmod +x /opt/stack
```

Grant the stack user `sudo` privileges:

```bash
echo "stack ALL=(ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/stack
```

Switch to the stack user:

```bash
sudo -u stack -i
```



### Installing this Repository

If you have your own OpenStack repository or a fork, you can configure DevStack to use it:

1. **Clone  Repository**:
   ```bash
   git clone https://github.com/Sergeant-ghost/openstack.git
   cd openstack
   ```

2. **Run DevStack**:
   ```bash
   ./stack.sh
   ```
3. **Access OpenStack**:
   - **Horizon**: `http://myhost/`
   - **Keystone**: `http://myhost/identity/v3/`
   - **CLI**: Source `openrc` and use OpenStack commands.

### Official Links

- [DevStack Documentation](https://docs.openstack.org/devstack/latest/)
- [OpenStack Official Site](https://www.openstack.org/)
- [My GitHub Repository](https://github.com/Sergeant-ghost/openstack.git)

### Customization

- **Configuration**: Modify `local.conf` for custom setups.
- **Stable Releases**: Use branches like `stable/zed` for specific versions.

### Notes

- **Root Access**: `stack.sh` requires `sudo` for certain tasks but should not be run as root.
- **User Account**: Use `tools/create-stack-user.sh` to set up the necessary user account.

### Official Links

- [DevStack Documentation](https://docs.openstack.org/devstack/latest/)
- [OpenStack Official Site](https://www.openstack.org/)

---

This version includes the supported OS versions and official links for further reference. Certainly! Here's the concise DevStack documentation with specified OS versions and official links for references.DevStack is a tool that deploys an OpenStack cloud for quick development and testing. This repository is a clone of the official OpenStack repository.

---
