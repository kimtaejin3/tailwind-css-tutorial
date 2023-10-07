# tailwind css 튜토리얼

## 필요한 명령어

`npx tailwindcss -i ./src/styles.css -o ./public/styles.css --watch`

## 초기세팅

```/** @type {import('tailwindcss').Config} */
//tailwind.config.json -> npx tailwind init
module.exports = {
  content: ["./public/**/*.{html,js}"],
  theme: {
    extend: {
      colors: {
        primary: "#ff6363",
        secondary: {
          100: "#e2e2d5",
          200: "#888883",
        },
      },
      fontFamily: {
        body: ["Dela Gothic One"],
      },
    },
  },
  plugins: [],
};
```

```
//package.json
 "scripts": {
    "build-css": "tailwindcss build src/styles.css -o public/styles.css"
  },
```

## 디렉토리 구성

```bash
├── public
│   ├── index.html
│   └── styles.css
├── src
│   └── styles.css
└── run.sh
```
