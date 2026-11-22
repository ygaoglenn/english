# Glenn's Daily English

网页地址：https://ygaoglenn.github.io/english/

## 文件夹结构

```
English/
├─ index.html             网页（主要改这个）
├─ manifest.webmanifest   App 名字、颜色、图标
├─ sw.js                  让网页能安装成 App、离线打开
├─ icons/                 App 图标
├─ app-key/               安卓 App 的安装包和签名钥匙（不会推到 GitHub）
├─ .gitignore             告诉 Git 哪些文件不要推
└─ README.md              本说明
```

## 更新网页

```
git add .
git commit -m "Update page"
git push
```

等 1–2 分钟，网页和手机 App 都会自动更新。

## 安卓 App

- 安装包在 `app-key/` 里的 zip 中（`Daily English.apk`）。
- 只有改 App 名字或图标时才需要重新生成 APK（PWABuilder → Package For Stores → Android → 选 "Use mine"，用 zip 里的 signing.keystore 和 signing-key-info.txt）。
- 钥匙丢了就不能覆盖安装，要卸载重装，打卡记录会清零。
