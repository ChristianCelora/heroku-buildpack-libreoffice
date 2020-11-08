# Heroku Buildpack for Libreoffice

Makes no assumptions about the LibreOffice version. Simply links the `.apt` binary into the `vendor` directory.

To be used in conjuction with  [heroku-buildpack-apt](https://github.com/heroku/heroku-buildpack-apt)

```
heroku buildpacks:add --index 1 https://github.com/heroku/heroku-buildpack-apt.git
heroku buildpacks:add --index 2 https://github.com/sumeetattree/heroku-buildpack-libreoffice.git
```

Create an `Aptfile` at the project root
```
libreoffice
libxinerama-dev
libgl1-mesa-dev
libglu1-mesa-dev
libxdamage-dev
libsm6
libice6
libharfbuzz0b
libharfbuzz-icu0
```
