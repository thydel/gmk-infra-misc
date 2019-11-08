# Import get-dup-pass.yml

```
src=~/usr/epipar.d/infra-plays
file=get-dup-pass.yml
git -C $src format-patch --stdout --root $file | git am -p1
echo tmp >> .gitignore
```

# Import named.yml

```
src=~/usr/thydel.d/infra-plays-19
file=named.yml
git -C $src format-patch --stdout --root $file | git am -p1
```
