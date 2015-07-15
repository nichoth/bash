# bash notes

List some directories and copy to clipboard all on one line

```bash
ls .. | grep something | tr '\n' ' ' | pbcopy
```

Get the basename for a file (remove the path):
    
    ${PATHNAME##*/}

for loop

```bash
for file in `ls`;
do
  echo "$file";
done
```

Create a file in each directory.

```bash
ls | xargs -I dir touch dir/text.txt
```

