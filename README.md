```
//1. gitignore 파일 만들기
npx gitignore node

// package.json 생성
yarn init --yes
```

- package.json에 types 추가
```
{
  "name": "ts-basics",
  "version": "1.0.0",
  "main": "dist/index.js",
  "types": "dist/index.d.ts",
  "license": "MIT"
}
```

- scripts
```  
"scripts": {
    "build": "tsc",
    "dev": "yarn build --watch --preserveWatchOuput"
    "lint": "eslint src ---ext js,ts",
    "test": "jest"    
}
```

- development dependency
```
yarn add -D typescript eslint jest
```

- volta로 node, yarn 고정