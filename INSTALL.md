# How to install daemontools

Like any other piece of software (and information generally), daemontools comes with NO WARRANTY.

## System requirements

daemontools works only under UNIX.

## Installation

Create a `/package` directory:

```shell
mkdir -p /package
chmod 1755 /package
cd /package
```

Download into `/package`. Unpack the daemontools package:

```shell
gunzip daemontools-X.XX.tar
tar -xpf daemontools-X.XX.tar
rm -f daemontools-X.XX.tar
cd daemontools-X.XX
```

Compile and set up the daemontools programs:

```shell
package/install
```

On BSD systems, reboot to start `svscan`.

To report success:

```shell
mail djb-sysdeps@cr.yp.to < /package/admin/daemontools/compile/sysdeps
```

