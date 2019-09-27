# Import get-dup-pass.yml

```
src=~/usr/epipar.d/infra-plays
file=get-dup-pass.yml
git -C $src format-patch --stdout --root $file | git am -p1
echo tmp >> .gitignore
```
