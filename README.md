# TS-in-GAS

GoogleAppScript project of TypeScript for local environment develop.

## How to pulling your GAS project in local repogitory and edit, push it.

```
  # If You havn't clasp, then please install it.
$ npm install -g @google/clasp

  # You should login.
$ clasp login

  # You can pulling your GAS project.
$ clasp clone { your_script_id }

  # Rename your GAS's コード.js to TypeScript file.
$ mv コード.js main.ts

  # You can push local environment editted content of your GAS.
$ clasp push
```

※ If you have failed `clasp push`, then You should chenge [settings about GAS API](https://script.google.com/home/usersettings) to on.

## If create `src/` directory.

```
  # Create src/ directory, and move 2 files to there.
$ mkdir src
$ mv {main.ts,appscript.json} src/
```

And You should add this 1 line to `.clasp.json` file.

```
{
    "scriptId": "{ your_script_id }"
    "roomDir": "./src"  // Please add this line.
}
```
