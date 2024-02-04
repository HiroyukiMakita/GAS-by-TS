# GAS-by-TS

GoogleAppScript projects of TypeScript for local environment develop.

## How to pulling your GAS project in local repogitory and edit, push it.

```
  # You should login.
$ yarn  clasp login

  # Make your GAS code put directory.
$ mkdir -p ./src/<dir_name>

  # You can pulling your GAS project.
$ yarn  clasp -P ./src/<dir_name> clone < your_script_id >
( If permission to access clasp is requested, grant it. )

  # Change your GAS code directory.
$ cd ./src/<dir_name>

  # Rename your GAS's コード.js to TypeScript file.
$ mv コード.js main.ts

  # You can push local environment editted content of your GAS.
$ yarn  clasp push
```

※ If you have failed `clasp push`, then You should chenge [settings about GAS API](https://script.google.com/home/usersettings) to on.
