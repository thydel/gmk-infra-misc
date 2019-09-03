# Fetch

```
git clone git@github.com:thydel/gmk-infra-misc.git
```

# Use a gmk file

```
gmk self/config
gmk mailmap
gmk conf
gmk exclude
gmk mailmaps
```

# Add and use a Makefile to generate inventory

```
make -f inventory.mk main
```

# Choose and configure ansible

```
make -C ext/ansible-cfg install
ansible-cfg median
source <(use-ansible)
ansible-cfg exclude
```

# Use ansible with inventory

```
source <(use-ansible)
ansible 'n_admin2:!g_poweredoff' -om ping
```
