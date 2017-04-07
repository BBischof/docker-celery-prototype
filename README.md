# docker_flask_germ
An essential setup for any docker deployed flask app with simple pytests.

## Mirroring to a new repo

For a new repo named `new_repository`:

Create the `new_repository` on [Github](https://github.com/new).

```(Bash)
mkdir scratch-dir; cd scratch-dir
# move to a scratch dir

git clone --bare https://github.com/BBischof/docker_flask_germ.git
# Make a bare clone of the repository

cd docker_flask_germ.git
git push --mirror https://github.com/BBischof/new_repository.git
# Mirror-push to the new repository

cd ..
rm -rf docker_flask_germ.git
# Remove our temporary local repository
```
