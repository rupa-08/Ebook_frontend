npm i -g typescript
npx react-native init Ebook_frontend --template react-native-template-typescript
npm install --save-dev babel-plugin-module-resolver

delete eslintrc.js
npm install --dev eslint prettier eslint-config-prettier
npm install eslint-config-prettier
npx eslint --init

eslint rules confilct with prettier
write prettier in eslintrc.json

# add this is package.json scripts

"build": "tsc",
"linter": "eslint 'src/**/\*.tsx'",
"prettier": "prettier --write 'src/**/\*.tsx'"

npm run linter = show error to those who are not using vs code
npm run prettier

Husky setup
npm install --dev husky
git should be initialized for this process
npx husky install
for precommit hook = npx husky add .husky/pre-commit "npm test"
