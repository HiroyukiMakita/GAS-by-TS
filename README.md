# GAS-by-TS

GoogleAppScript projects of TypeScript for local environment develop.

## How to pulling your GAS project in local repository and edit, push it

```bash
  # You should login.
$ yarn clasp login

  # Make your GAS code put directory.
$ mkdir -p ./src/<dir_name>

  # You can pulling your GAS project.
$ yarn clasp -P ./src/<dir_name> clone < your_script_id >
( If permission to access clasp is requested, grant it. )

  # Rename your GAS's コード.js to TypeScript file.
$ mv ./src/<dir_name>/コード.js ./src/<dir_name>/main.ts

  # You can push local environment edited content of your GAS.
$ yarn clasp  -P ./src/<dir_name> push
```

※ If you have failed `clasp push`, then You should change [settings about GAS API](https://script.google.com/home/usersettings) to on.
