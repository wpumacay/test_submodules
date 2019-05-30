# test_submodules
Just a test of some submodules

## Testing shallow clones

If you clone recursively, you will grab all contents of the submodules
without specifying depth (no shallow)

```shell
git clone --recursive https://github.com/wpumacay/test_submodules.git
```

To avoid this, just clone without initializing the submodule, and then
update it appropriately.

```shell
# Clone without recursive
git clone https://github.com/wpumacay/test_submodules.git

# Update submodules using shallow update
git submodule update --init --depth 1
```

