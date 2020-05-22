# **react-app-starter**


**visual studio code - create-react-app - eslint - prettier - husky - lint-staged**

<br />

---
## **ESlint**

1. ### Delete default cra eslint configuration

```json
  "eslintConfig": {
    "extends": "react-app"
  }
```

<br />

2. ### Instal VSCode Plugin

<https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint>


<br />

3. ### Install eslint

```npm install eslint --save-dev```

<br />

4. ### Install eslint airbnb config

```npx install-peerdeps --dev eslint-config-airbnb```

<br />

5. copy **.eslintrc** file to main folder

<br />

---
## **Prettier**

1. ### Instal VSCode Plugin

<https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode>

<br />

2. ### Install prettier

```npm install prettier --save-dev```

<br />

3. ### Install prettier eslint config

```npm install eslint-config-prettier --save-dev```

<br />

4. copy **.prettierrc** file to main folder

<br />

---
## **Lint staged**

1. ### Instal lint-staged

```npm install lint-staged --save-dev```

<br />

2. ### Add to pacakge.json

```json
  "lint-staged": {
    "*.js": [
      "prettier --config .prettierrc --write",
      "eslint --fix",
      "git add"
    ]
  }
```

<br />

---
## **Husky**

1. ### Instal husky

```npm install husky --save-dev```

<br />

2. ### Add to pacakge.json

```json
  "husky": {
    "hooks": {
      "pre-commit": "lint-staged"
    }
  }
```

&copy;Tomasz Kowalczyk
