# Onboarding Shit

Why do you want to work here? That's dumb. Even I don't want to work here, and I helped found this place.

## Linters and Formatters
1. Go fuck yourself.

After that's out of the way, set the following shit up in your [vscode editor](https://code.visualstudio.com/download).
Notice how I didn't say "in your preferred editor"? That's because we have _standards_.

2. Install Linters
    - **ESLint** (extension ID: dbaeumer.vscode-eslint)
    - **Flake8** (extension ID: ms-python.flake8)
3. Install Formatters
    - **Prettier** (extension ID: esbenp.prettier-vscode)
    - **Black** (extension ID: ms-python.black-formatter)
    - **isort** (extension ID: ms-python.isort)

If it wasn't completely fuckin' obvious, you just installed a linter/formatter combo (and an imports sorter) to cover both the frontend and backend projects we support.

4. Update VSCode User Settings
    - `Press ⌘ + shift + P on Mac`
    - Search and select "user settings (json)"
    - add the following custom settings
    ```json
    "typescript.updateImportsOnFileMove.enabled": "always",
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "prettier.requireConfig": true,
    "editor.formatOnSave": true,
    "editor.formatOnPaste": true,
    "[python]": {
      "editor.defaultFormatter": "ms-python.black-formatter",
      "editor.formatOnSave": true,
      "editor.codeActionsOnSave": {
        "source.organizeImports": true
      }
    },
    "isort.args": ["--profile", "black"]
    ```

5. Install Optionals
    - **Django** (extension ID: batisteo.vscode-django)
    - **Git Blame** (extension ID: waderyan.gitblame)
    - **Git History** (extension ID: donjayamanne.githistory)
    - **Python** (extension ID: ms-python.python)
    - **ES7+** (extension ID: dsznajder.es7-react-js-snippets)
    - **Codeium** (extension ID: Codeium.codeium)

6. Restart VSCode for the fun of it

Now you're standardized, and the shit code you push should be a little less shitty. This setup should format code on save / paste and lint code for any problems that your dumbass definitely missed. If you installed the optionals, this setup should also suggest AI-powered code snippets, highlight code in useful ways, and even let you know what dumbass broke the line you're fixing so you can make them feel bad about it.

**Welcome!!**
