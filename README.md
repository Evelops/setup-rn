# RN Firebase Test App

</hr>

> Basic Info

```
BUNDLE IDENTIFIER -> com.gcc.billapp
APP_NAME -> billRnApp
```

<br>

> react-native-rename[https://github.com/junedomingo/react-native-rename#readme]

</hr>

</br>

```
# first add your repository and then follow contents
# and each paractice your finish plz commit & push your repository

$ git checkout -b rename-app
$ yarn add react-native-rename
$ npx react-native-rename "test-app"
$ npx react-native-rename "test-app" -b "com.gcc.test-app" # com.google.test-app
```

<br>

> react-native-firebase/app[https://rnfirebase.io/]

</hr>

<br>

```
# 1. yarn add @react-native-firebase/app
2a. setup -> android setup ( add key )
2b. setup -> ios setup ( add key )

#still need firestore

$ yarn add @react-native-firebase/firestore

#adding auth

$ yarn add @react-native-firebase/auth

# pod install !!!!!!!
$ npx pod-install

```

</br>

> Setup eslint-prettier-husky[https://dev-yakuza.posstree.com/en/react-native/eslint-prettier-husky-lint-staged/]

</hr>

<br>

> ## setting up eslint-prettier-husky[https://dev-yakuza.posstree.com/en/react-native/eslint-prettier-husky-lint-staged/]

</hr>

```
1. yarn add eslint -D



2. npx eslint --init

   링크에 나온것처럼 설치할것 마지막 것은 no로 선택하고 아래 3번으로 다시 할것



- answer questions like link



3. yarn add -D eslint-plugin-react @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-plugin-react-hooks



4.eslintrc.js 파일을 링크에 나오는것 처럼 수정한다.

modify .eslintrc.js - like link



5.package.json 에 scripts 부분에 "lint": "eslint --ext .tsx --ext .ts src/" 추가

add scripts for lint in package.json - "lint": "eslint --ext .tsx --ext .ts src/",



6. src 폴더 만들고 App.tsx 파일 만들기



7. 에러가 생긴다면 npx eslint ./src/\*_/_.tsx --fix 한번 해주기

8.tsconfig.json 파일에 "include": ["./.eslintrc.js", "./src/**/*"] 추가하기

yarn add -D eslint-plugin-prettier eslint-config-prettier


add prettier

1. yarn add -D prettier eslint-plugin-prettier

2. package.json의 scripts에 "format": "prettier --check ./src" 추가하기

3. add husky

   yarn add -D husky
   yarn add -D lint-staged


4. package.json 아래부분에 추가

   {

   ...

   "lint-staged": {

   "src/**/\*.{ts,tsx}": [

   "eslint --ext .tsx --ext .ts src/ --fix"

   ],

   "./src/**": [

   "prettier --write ."

   ]

   },

   "husky": {

   "hooks": {

   "pre-commit": "lint-staged"

   }

   },
   ...

   }
```

<br>

> react-native-magnus

```
yarn add react-native-magnus
yarn add react-native-animatable react-native-modal react-native-vector-icons

```

> react-navigation[https://reactnavigation.org/docs/getting-started/]

```
yarn add @react-navigation/native

yarn add react-native-screens react-native-safe-area-context

npx pod-install ios

react-native-screens package requires one additional configuration step to properly work on Android devices. Edit MainActivity.java file which is located in android/app/src/main/java/<your package name>/MainActivity.java.

Add the following code to the body of MainActivity class:

@Override
protected void onCreate(Bundle savedInstanceState) {
  super.onCreate(null);
}

and make sure to add an import statement at the top of this file:

import android.os.Bundle;

yarn add @react-navigation/native-stack

yarn add @react-navigation/bottom-tabs

-- Material Tab Tabs

https://reactnavigation.org/docs/material-top-tab-navigator#installation

yarn add @react-navigation/material-top-tabs react-native-tab-view

yarn add react-native-pager-view


for some ui elements or types
yarn add @react-navigation/elements
```

</br>

> react-native-async-storage/async-storage

```
yarn add @react-native-async-storage/async-storage
npx pod-install
```
