## Git repo for educational purposes


```shell
git lfs install
```


### Create repo from scratch

```shell
git init . && \
git lfs install && \
git config --add user.email "it@trianglesis.org.ua" && \
git config --add user.name "Oleksandr D" && \
git lfs track "*.zip" && \
git lfs track "*.xz" && \
git lfs track "*.gz" && \
git lfs track "*.dml" && \
git lfs track "*.dmltemp" && \
git lfs track "*.model" && \
git lfs track "*.log" && \
git lfs track "*.rpm" && \
git lfs track "*.mp4" && \
git lfs track "*.pdf" && \
git remote add origin git@github.com:trianglesis/git_ed_piblic.git && \
git add README.md && \
git add .gitattributes && \
git add .gitignore && \
git commit -m "first commit" && \
git branch -M main && \
git push -u origin main && \
echo "Git config finish!"
```


### Always fix line endings for everyone:

- https://docs.github.com/en/get-started/getting-started-with-git/configuring-git-to-handle-line-endings


### At local system:

```shell
git config --global core.autocrlf true
```


### At repo for all

```
vi .gitattributes
```

```shell
# Set the default behavior, in case people don't have core.autocrlf set.
* text=auto

# Explicitly declare text files you want to always be normalized and converted
# to native line endings on checkout.
*.py text
*.tplpre text
*.dml text
*.dmltemp text
*.model text
```



# Other useful links:

## Ignore files and folders:

- https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files


## Git Cheat Sheets:

- https://training.github.com/

