# Init local repo

```
git init gmk-infra-misc
```

Then works from the new repo

# Init gmk

```
edit boot.yml
gmk file=boot init
```

# Create github repo

```
gmk file=boot self/create
```

Will display the cmd to run

# Add files to repos and make first commit

```
git add .
git ci -m 'First commit'
git push --set-upstream origin master
```

# Add and use a gmk file

```
gmk self/config
gmk mailmap
gmk conf
gmk mailmaps
```

# Add and use a Makefile to generate inventory

```
make -f inventory main
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
