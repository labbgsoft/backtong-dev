# hmm_backtong_v2_vuejs

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### 배포

#### 윈도우 최대화 최소화 옵션 활성화

​	웹 브라우져에서 디버깅을 위해서 `npm run serve`로 사용할 경우 주석처리 해주어야하고, 배포를 하거나 `npm run electron:serve`를 하여 디버깅할 경우 추석을 해제한다.

* DefaultContainer.vue

  ```javascript
  import { electron, remote, BrowserWindow } from 'electron';
  const window = remote.BrowserWindow.getFocusedWindow();
  ```

* Login.vue

  ```javascript
  import { remote } from 'electron';
  const window = remote.BrowserWindow.getFocusedWindow()
  ```

  

* package.json 의 버전 수정 
* 빌드 및 업로드 
```
npm run publish
```
* 릴리즈 
 ** https://github.com/labbgsoft/bacttong/releases 이동후 릴리즈로 해당 버전 수정

 