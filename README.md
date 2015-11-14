# Day For Night

Hackpad: https://fallsfpc2015.hackpad.com/Day-4-Night-e6Zo9q7mBAs

## Contributing

This project requires **openFrameworks 0.9.0**. You can [download it from the oF website](http://openframeworks.cc/download/) if you don't already have it installed.






### Development Setup

It's probably a good idea to work in your own branch. Create a new branch:

```bash
git checkout -b branchName
```

Now you can use the project generator script to generate a new scene. This will copy the `emptyScene` files and rename based on your new scene name.

Use the terminal to `cd` into your project folder and run the following, substituting `sceneName` with the name of your scene:

```bash
./generate_scene.sh sceneName
```

It will copy the following files and create new files for your new scene:

`bin/data/emptyScene/` => `bin/data/sceneName/`
`src/scenes/emptyScene/ => `src/scenes/sceneName/`


### Submitting Changes

#### If you're adding a new scene and not changing the architecture

Check to make sure you don't have uncommitted changes (commit them if you do):

```bash
git status
```

Now checkout the master branch and make sure it's up to date:

```bash
git checkout master
git pull
```

Now merge in your branch:

```bash
git merge branchName
```

Now push your changes to the repo:

```bash
git push
```


#### If you're making architectural changes

It's probably better to push your branch instead of merging directly into `master`, then submit a pull request.

Check to make sure you don't have uncommitted changes in your branch (commit them if you do):

```bash
git status
```
Now push your branch to GitHub:

```bash
git push origin branchName
```

Now [go to GitHub repo](https://github.com/ofZach/dayForNightSFPC) and submit a pull request via the GH interface.