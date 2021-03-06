[![hp](https://raw.githubusercontent.com/moyomogi/rvw2022s/master/docs/hp.svg)](https://rvw2022s.herokuapp.com)
[![last-commit](https://img.shields.io/github/last-commit/moyomogi/rvw2022s)](https://github.com/moyomogi/rvw2022s/commits/master)
[![license](https://img.shields.io/badge/license-CC0-blue)](https://creativecommons.org/publicdomain/zero/1.0/deed.ja)

# Random Virtual World 2022 ð¸
<img src="https://i.imgur.com/R9YV2YX.png" width="180">  

## ã¤ã³ã¹ãã¼ã«
WSL ã®ä¸ã§ä½æ¥­ãã¦ãã ããã  
ã¾ãç·è²ã® `Code > Download ZIP` ãã DL ãã¦ãå¥½ããªå ´æã«ç½®ãã¦ãã ããããã®å¾ãã«ã¬ã³ããã©ã«ãã§ä¸è¨ã³ãã³ããå®è¡ãã¦ãã ããã  
```sh
# ./package.json ã® "dependencies", "devDependencies" ã«ããã³ãã³ããã¤ã³ã¹ãã¼ã«
npm install
```

## localhost ã«ãµã¼ãããæ¹æ³
### éçºã¢ã¼ãã§ãµã¼ã
[localhost:3000](http://localhost:3000) ã«ã¦ãµã¼ããããã
```sh
# ./package.json ã® "scripts" ã® "dev" ã«ããã³ãã³ããå®è¡ãããã®æ
npm run dev
```

### è£½åã¢ã¼ãã»Node.js hosting (Heroku ãªã©) ã¢ã¼ãã§ãµã¼ã
[localhost:3000](http://localhost:3000) ã«ã¦ãµã¼ããããã
Heroku ã«ããã­ã¤ãã¦ããã®ã§ãä»åã¯ãã£ã¡ã
```sh
npm run build
npm run start
```

### (è£½åã¢ã¼ãã»Static hosting (GH Pages ãªã©) ã¢ã¼ãã§ãµã¼ã)
[localhost:3000](http://localhost:3000) ã«ã¦ãµã¼ããããã
```sh
# dist ãã©ã«ãã«ãã¡ã¤ã«ç¾¤ãçæ
npm run generate
# localhost ã«ã¦ãµã¼ããã
npm run start
```

## Firestore, Firebase Storage ã®è¨­å®
è©³ããã¯ [Firebaseã§ããã­ã¤ãããï¼](https://qiita.com/hiroki-harada/items/ca22ac177db68e3c3796) ãåç§ã
```sh
# `firebase` ã³ãã³ãã®ã¤ã³ã¹ãã¼ã«
npm install -g firebase-tools
# Firebase ã«ã­ã°ã¤ã³
firebase login
```

## Heroku ã«ããã­ã¤
### ååè¨­å®
ã¢ã«ã¦ã³ããä½ã£ãå¾ãå¬å¼è§£èª¬ [Getting Started on Heroku with Node.js](https://devcenter.heroku.com/articles/getting-started-with-nodejs) ã«å¾ããä»¥ä¸ãå®è¡ã
```sh
heroku login
# `rvw2022s` ã¯èªåã® Heroku ãã­ã¸ã§ã¯ãåã«å¤æ´ãã¦ãã ãã
heroku git:remote -a rvw2022s
```

### ä»¥éã¯ãããå®è¡
```sh
git add --all
git commit -m "Test heroku"
git push heroku master  # Heroku ã«ããã­ã¤
# git push origin master  # Github ã«ããã­ã¤
```

## æè¡ã¹ã¿ãã¯
- [NuxtJS](https://nuxtjs.org/ja/docs/get-started/installation/)
  Vue.js ã®ãã¬ã¼ã ã¯ã¼ã¯
- [Tailwind CSS](https://tailwindcss.com/docs/installation)
  `/` ã­ã¼ãæ¼ãã¨ãã¯ã©ã¹ã§æ¤ç´¢ã§ãã¾ãã
- [@nuxtjs/tailwindcss](https://tailwindcss.nuxtjs.org)
  NuxtJS ã¢ããªã±ã¼ã·ã§ã³ã« Tailwind CSS ãæè»½ã«å°å¥ã§ããã
- [Firebase](https://firebase.google.com/)
  Firestore, Firebase Storage ã DB ã¨ãã¦ä½¿ã£ã¦ãã¾ãã
- [Heroku](https://jp.heroku.com/)
  Node.js hosting ã§ãã Heroku ã§ãã¹ãã£ã³ã°ãã¦ãã¾ãã
- [vue-awesome-swiper](https://web.archive.org/web/20211127071455/https://github.surmon.me/vue-awesome-swiper/)
  ã¹ã©ã¤ãã·ã§ã¼æ©è½

## åèæç®
- [Making a Navigation Drawer/Sliding Sidebar with TailwindCSS](https://dev.to/fayaz/making-a-navigation-drawer-sliding-sidebar-with-tailwindcss-blueprint-581l)
  `components/TheNavbar.vue` ã§ä½¿ãã¾ããã
- [Multi Section Form | Tailwind Toolbox](https://www.tailwindtoolbox.com/templates/multi-section-form)
  `pages/submit.vue`, `pages/update.vue` ã§ä½¿ãã¾ããã
- [Tailblocks](https://tailblocks.cc)
  `components/TheSlides.vue` ã§ä½¿ãã¾ããã

## License
ãããã®ã³ã¼ãã¯ [CC0](https://creativecommons.org/publicdomain/zero/1.0/deed.ja) ã§è¨±è«¾ããã¦ãã¾ããããªãã¡ãåç¨å©ç¨ã»éåç¨å©ç¨ãåãããå¼ç¨åã«è¨è¼ããã«ããããã®ã³ã¼ãã®ä¸é¨ã¾ãã¯å¨é¨ãä½¿ç¨ã§ãã¾ãã
