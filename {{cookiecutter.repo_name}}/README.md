# Amoskeag KiCAD libraries

## Add to your project

To add into your project

```
git submodule add https://github.com/{{cookiecutter.github}}/{{cookiecutter.repo_name}}.git
```

## 3D Models

open `Preferences` and `Configure Paths` then add the following enviorment variable:

```
Name: AMOSKEAG_3DMODELS
Path: <Path to folder>
```


## Kibot

And if you use kibot, add this to your `pre_flight`

```
preflight:
  ...
  set_text_variables:
    - name: "AMOSKEAG_3DMODELS" # 3D models for Amoskeag Library
      command: "echo 'Hardware/Board/Libraries/Amoskeag_KiCAD_Libs/3D'"
```

# Projects using this lib:

