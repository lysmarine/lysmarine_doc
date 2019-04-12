
# lysmarine-gen (the build script for the lysmarine image)
```
git clone https://gitlab.com/lysmarine/lysmarine-gen.git
cd lysmarine-gen
sudo CLEAN=1 ./build.sh
```

Then you can find the image file at location `work/xxx-lysmarine/export-noobs/`


Development should be done in the `develop` branch

Change the branch with `git checkout develop`


New version [Release procedure](doc/procedures/release_procedure.md)


# Build Lysmarine (The documentation website)


## Run the documentation website

The doc for lysmarine is generated with http://docsify.js.org

To use it locally, First install docsify package from npm:
```
  sudo npm i docsify-cli -g
```

Then, download lysmarine documentation.
```
https://gitlab.com/lysmarine/lysmarine.git
cd lysmarine
```


To serve the documentation site:
```
  docsify serve ./
```
Now you should be able to access documentation on `http://localhost:3000`
