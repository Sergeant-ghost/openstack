Certainly! Here's the concise DevStack documentation with specified OS versions and official links for references:

---

### DevStack Quick Start

DevStack is a tool to quickly deploy an OpenStack cloud for development and testing.

#### Goals

- Quickly build OpenStack environments in Ubuntu or RockyLinux.
- Facilitate OpenStack development and testing.

#### Important

- **Use a VM**: Run `stack.sh` in a clean, disposable VM to avoid altering your main system.

### Supported OS Versions

- **Ubuntu**: [20.04 LTS (Focal Fossa)](https://releases.ubuntu.com/20.04/) or [22.04 LTS (Jammy Jellyfish)](https://releases.ubuntu.com/22.04/)
- **Rocky Linux**: [8.x](https://rockylinux.org/download) or [9.x](https://rockylinux.org/download)

### Installation Steps

1. **Clone DevStack Repository**:
   ```bash
   git clone https://opendev.org/openstack/devstack.git
   cd devstack
   ```

2. **Create and Configure `local.conf`**:
   ```bash
   cp samples/local.conf .
   ```
   - Set passwords and customize options in `local.conf`.

3. **Run DevStack**:
   ```bash
   ./stack.sh
   ```

4. **Access OpenStack**:
   - **Horizon**: `http://myhost/`
   - **Keystone**: `http://myhost/identity/v3/`
   - **CLI**: Source `openrc` and use OpenStack commands.

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

This version includes the supported OS versions and official links for further reference.Certainly! Here's the concise DevStack documentation with specified OS versions and official links for references:

---

### DevStack Quick Start

DevStack is a tool to quickly deploy an OpenStack cloud for development and testing.

#### Goals

- Quickly build OpenStack environments in Ubuntu or RockyLinux.
- Facilitate OpenStack development and testing.

#### Important

- **Use a VM**: Run `stack.sh` in a clean, disposable VM to avoid altering your main system.

### Supported OS Versions

- **Ubuntu**: [20.04 LTS (Focal Fossa)](https://releases.ubuntu.com/20.04/) or [22.04 LTS (Jammy Jellyfish)](https://releases.ubuntu.com/22.04/)
- **Rocky Linux**: [8.x](https://rockylinux.org/download) or [9.x](https://rockylinux.org/download)

### Installation Steps

1. **Clone DevStack Repository**:
   ```bash
   git clone https://opendev.org/openstack/devstack.git
   cd devstack
   ```

2. **Create and Configure `local.conf`**:
   ```bash
   cp samples/local.conf .
   ```
   - Set passwords and customize options in `local.conf`.

3. **Run DevStack**:
   ```bash
   ./stack.sh
   ```

4. **Access OpenStack**:
   - **Horizon**: `http://myhost/`
   - **Keystone**: `http://myhost/identity/v3/`
   - **CLI**: Source `openrc` and use OpenStack commands.

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

This version includes the supported OS versions and official links for further reference.
