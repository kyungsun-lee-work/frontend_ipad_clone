[![Netlify Status](https://api.netlify.com/api/v1/badges/d07cf9d9-8012-4144-ba84-a8af40458941/deploy-status)](https://app.netlify.com/sites/transcendent-naiad-733465/deploys)

# ๐ iPad

iPad product page clone development.

[DEMO](https://fascinating-blancmange-dfe59f.netlify.app)

![Screenshots](./images/screenshot1.jpg)

### Reset.css

Initialize browser's style.

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css"
/>
```

### Google Fonts

English: [Roboto](https://fonts.google.com/specimen/Roboto)
Korean: [Noto Sans KR](https://fonts.google.com/noto/specimen/Noto+Sans+KR)

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;700&family=Roboto:wght@400;500;700&display=swap"
  rel="stylesheet"
/>
```

### Open Graph and Twitter Card

```html
<!--Open Graph-->
<meta property="og:type" content="website" />
<meta property="og:site_name" content="Apple (KR)" />
<meta property="og:title" content="iPad 10.2" />
<meta
  property="og:description"
  content="๊ฐ๋ ฅํ A13 Bionic ์นฉ์ ํ์ฌํ iPad. ์ผํฐ ์คํ์ด์ง ๊ธฐ์ ์ด ์ ์ฉ๋ 12MP ์ธํธ๋ผ ์์ด๋ ์ ๋ฉด ์นด๋ฉ๋ผ, True Tone ๋์คํ๋ ์ด ๊ธฐ์  ๋ฐ 64GB ์ ์ฅ ์ฉ๋๊น์ง ๊ฐ์ท์ต๋๋ค."
/>
<meta property="og:image" content="./images/ipad-seo.png" />
<meta property="og:url" content="https://www.apple.com/kr/ipad-10.2/" />

<!--Twitter Card-->
<meta property="twitter:card" content="summary" />
<meta property="twitter:site" content="Apple (KR)" />
<meta property="twitter:title" content="iPad 10.2" />
<meta
  property="twitter:description"
  content="๊ฐ๋ ฅํ A13 Bionic ์นฉ์ ํ์ฌํ iPad. ์ผํฐ ์คํ์ด์ง ๊ธฐ์ ์ด ์ ์ฉ๋ 12MP ์ธํธ๋ผ ์์ด๋ ์ ๋ฉด ์นด๋ฉ๋ผ, True Tone ๋์คํ๋ ์ด ๊ธฐ์  ๋ฐ 64GB ์ ์ฅ ์ฉ๋๊น์ง ๊ฐ์ท์ต๋๋ค."
/>
<meta property="twitter:image" content="./images/ipad-seo.png" />
<meta property="twitter:url" content="https://www.apple.com/kr/ipad-10.2/" />
```

### Hero Contents

```html
<p class="pricing">โฉ449,000๋ถํฐ</p>
```

### CSS Variables

```css
html {
  --color-white: #fff;
  --color-black: #000;
  --color-font: #1d1d1d;
  --color-font-darkgray: #6e6e6e;
  --color-font-middlegray: #b7b7b7;
  --color-font-lightgray: #f5f5f5;
  --color-link: #0071e3;
  --color-link-focus: #81b9f1;
  --color-border: #d2d2d2;
  --color-header: #3a3a3a;
  --color-section: #f5f5f5;
  --color-shadow: rgba(0, 0, 0, 0.4);
}
.example {
  background-color: var(--color-font);
}
```

### Icons

```css
.info .icon.icon--chip {
  background-image: url("../images/sprite_chip.png");
}
.info .icon.icon--faster {
  background-image: url("../images/sprite_faster.png");
}
.info .icon.icon--neural {
  background-image: url("../images/sprite_neural.png");
}
.info .icon.icon--apps {
  background-image: url("../images/sprite_apps.png");
}
.info .icon.icon--battery {
  background-image: url("../images/sprite_battery.png");
}
.info .icon.icon--display {
  background-image: url("../images/sprite_display.png");
}
.info .icon.icon--true-tone {
  background-image: url("../images/sprite_true_tone.png");
}
.info .icon.icon--center-stage {
  background-image: url("../images/sprite_center_stage.png");
}
.info .icon.icon--front-camera {
  background-image: url("../images/sprite_front_camera.png");
}
.info .icon.icon--back-camera {
  background-image: url("../images/sprite_back_camera.png");
}
.info .icon.icon--scan {
  background-image: url("../images/sprite_scan.png");
}
.info .icon.icon--download {
  background-image: url("../images/sprite_download.png");
}
.info .icon.icon--wifi {
  background-image: url("../images/sprite_wifi.png");
}
.info .icon.icon--lte {
  background-image: url("../images/sprite_lte.png");
}
.info .icon.icon--pencil {
  background-image: url("../images/sprite_pencil.png");
}
.info .icon.icon--keyboard {
  background-image: url("../images/sprite_keyboard.png");
}
.info .icon.icon--notes {
  background-image: url("../images/sprite_notes.png");
}
.info .icon.icon--covers {
  background-image: url("../images/sprite_covers.png");
}
```

### Sprite Icon Animation

<img src="./images/sprite_apps.png" alt="์ด๋ฏธ์ง ์คํ๋ผ์ดํธ" width="300" />

```css
@keyframes sprite-icon {
  /* 1~10 */
  0.00% {
    background-position: 0 0;
  }
  1.67% {
    background-position: -100px 0;
  }
  3.33% {
    background-position: -200px 0;
  }
  5.00% {
    background-position: -300px 0;
  }
  6.67% {
    background-position: -400px 0;
  }
  8.33% {
    background-position: -500px 0;
  }
  10.00% {
    background-position: 0 -100px;
  }
  11.67% {
    background-position: -100px -100px;
  }
  13.33% {
    background-position: -200px -100px;
  }
  15.00% {
    background-position: -300px -100px;
  }

  /* 11~20 */
  16.67% {
    background-position: -400px -100px;
  }
  18.33% {
    background-position: -500px -100px;
  }
  20.00% {
    background-position: 0 -200px;
  }
  21.67% {
    background-position: -100px -200px;
  }
  23.33% {
    background-position: -200px -200px;
  }
  25.00% {
    background-position: -300px -200px;
  }
  26.67% {
    background-position: -400px -200px;
  }
  28.33% {
    background-position: -500px -200px;
  }
  30.00% {
    background-position: 0 -300px;
  }
  31.67% {
    background-position: -100px -300px;
  }

  /* 21~30 */
  33.33% {
    background-position: -200px -300px;
  }
  35.00% {
    background-position: -300px -300px;
  }
  36.67% {
    background-position: -400px -300px;
  }
  38.33% {
    background-position: -500px -300px;
  }
  40.00% {
    background-position: 0 -400px;
  }
  41.67% {
    background-position: -100px -400px;
  }
  43.33% {
    background-position: -200px -400px;
  }
  45.00% {
    background-position: -300px -400px;
  }
  46.67% {
    background-position: -400px -400px;
  }
  48.33% {
    background-position: -500px -400px;
  }

  /* 31~40 */
  50.00% {
    background-position: 0 -500px;
  }
  51.67% {
    background-position: -100px -500px;
  }
  53.33% {
    background-position: -200px -500px;
  }
  55.00% {
    background-position: -300px -500px;
  }
  56.67% {
    background-position: -400px -500px;
  }
  58.33% {
    background-position: -500px -500px;
  }
  60.00% {
    background-position: 0 -600px;
  }
  61.67% {
    background-position: -100px -600px;
  }
  63.33% {
    background-position: -200px -600px;
  }
  65.00% {
    background-position: -300px -600px;
  }

  /* 41~50 */
  66.67% {
    background-position: -400px -600px;
  }
  68.33% {
    background-position: -500px -600px;
  }
  70.00% {
    background-position: 0 -700px;
  }
  71.67% {
    background-position: -100px -700px;
  }
  73.33% {
    background-position: -200px -700px;
  }
  75.00% {
    background-position: -300px -700px;
  }
  76.67% {
    background-position: -400px -700px;
  }
  78.33% {
    background-position: -500px -700px;
  }
  80.00% {
    background-position: 0 -800px;
  }
  81.67% {
    background-position: -100px -800px;
  }

  /* 51~60 */
  83.33% {
    background-position: -200px -800px;
  }
  85.00% {
    background-position: -300px -800px;
  }
  86.67% {
    background-position: -400px -800px;
  }
  88.33% {
    background-position: -500px -800px;
  }
  90.00% {
    background-position: 0 -900px;
  }
  91.67% {
    background-position: -100px -900px;
  }
  93.33% {
    background-position: -200px -900px;
  }
  95.00% {
    background-position: -300px -900px;
  }
  96.67% {
    background-position: -400px -900px;
  }
  98.33% {
    background-position: -500px -900px;
  }
}
```

```js
let x = 0;
let y = 0;
let frames = "";
for (let i = 0; i < 60; i += 1) {
  frames += `${((100 / 60) * i).toFixed(2)}% { background-position: ${x}${
    x === 0 ? "" : "px"
  } ${y}${y === 0 ? "" : "px"}; }\n`;
  if (x <= -500) {
    x = 0;
    y -= 100;
    continue;
  }
  x -= 100;
}
// document.body.innerHTML = frames
console.log(frames);
```

### IntersectionObserver

[IntersectionObserver](https://heropy.blog/2019/10/27/intersection-observer/)

```js
const io = new IntersectionObserver((entries) => {
  entries.forEach((entry) => {
    if (!entry.isIntersecting) {
      return;
    }
    entry.target.classList.add("show");
  });
});

const infoEls = document.querySelectorAll(".info");
infoEls.forEach((el) => io.observe(el));
```

### iPad products

```js
export default [
  {
    thumbnail: "./images/compare_ipad_pro.png",
    colors: ["#68696D", "#E2E3E5"],
    name: "iPad Pro",
    tagline: "๊ถ๊ทน์ iPad๋<br />์ด๋ฐ ๊ฒ.",
    price: 999000,
    url: "/ipad-pro/",
  },
  {
    thumbnail: "./images/compare_ipad_air.png",
    colors: ["#68696D", "#E2E3E5", "#E8D2CE", "#B9B8D1", "#88AEBF"],
    name: "iPad Air",
    tagline: "๊ฐ๋ ฅํ๋ค. ๋ค์ฑ๋กญ๋ค.<br />๊ฒฝ์ด๋กญ๋ค.",
    price: 779000,
    url: "/ipad-air/",
  },
  {
    thumbnail: "./images/compare_ipad_10_2.png",
    colors: ["#68696D", "#E2E3E5"],
    name: "iPad",
    tagline: "๋ง์กฑ์ค๋ฌ์ด ์ฑ๋ฅ.<br />๊ธฐ๋ถ ์ข์ ๊ฐ๊ฒฉ.",
    price: 449000,
    url: "/ipad-10.2/",
  },
  {
    thumbnail: "./images/compare_ipad_mini.png",
    colors: ["#68696D", "#E2E3E5", "#E8D2CE", "#B9B8D1"],
    name: "iPad Pro",
    tagline: "๋ฉ๊ฐ๊ธ ์ฑ๋ฅ.<br />ํฌ๊ธฐ๋ง ๋ฏธ๋.",
    price: 649000,
    url: "/ipad-mini/",
  },
];
```

### Footer

```js
export default [
  {
    title: "์ผํ ๋ฐ ์์๋ณด๊ธฐ",
    maps: [
      { name: "์คํ ์ด", url: "/shop/goto/store" },
      { name: "Mac", url: "/mac" },
      { name: "iPad", url: "/ipad" },
      { name: "iPhone", url: "/iphone" },
      { name: "Watch", url: "/watch" },
      { name: "AirPods", url: "/airpods" },
      { name: "TV ๋ฐ ํ", url: "/tv-home" },
      { name: "AirTag", url: "/airtag" },
      { name: "์ก์ธ์๋ฆฌ", url: "/shop/goto/buy_accessories" },
    ],
  },
  {
    title: "์๋น์ค",
    maps: [
      { name: "Apple Music", url: "/apple-music" },
      { name: "Apple TV+", url: "/apple-tv-plus" },
      { name: "Apple Arcade", url: "/apple-arcade" },
      { name: "iCloud", url: "/icloud" },
      { name: "Apple Books", url: "/apple-books" },
      { name: "Apple Podcast", url: "/apple-podcasts" },
      { name: "App Store", url: "/app-store" },
    ],
  },
  {
    title: "๊ณ์ ",
    maps: [
      { name: "Apple ID ๊ด๋ฆฌ", url: "https://appleid.apple.com" },
      { name: "Apple Store ๊ณ์ ", url: "/shop/goto/account" },
      { name: "iCloud.com", url: "https://www.icloud.com" },
    ],
  },
  {
    title: "Apple Store",
    maps: [
      { name: "๋งค์ฅ ์ฐพ๊ธฐ", url: "/retail" },
      { name: "Genius Bar", url: "/retail/geniusbar" },
      { name: "Today at Apple", url: "/today" },
      { name: "Apple ์บ ํ", url: "/today/camp" },
      {
        name: "Apple Store ์ฑ",
        url: "https://apps.apple.com/app/apple-store/id375380948",
      },
      { name: "๋ฆฌํผ ๋ฐ ํน๊ฐ ์ ํ", url: "/shop/goto/special_deals" },
      { name: "๊ธ์ต ํํ", url: "/shop/goto/financing" },
      { name: "Apple Trade In", url: "/trade-in" },
      { name: "์ฃผ๋ฌธ ์ํ", url: "/shop/goto/order/list" },
      { name: "์ผํ ๋์๋ง", url: "/shop/goto/help" },
    ],
  },
  {
    title: "๋น์ฆ๋์ค",
    maps: [
      { name: "Apple๊ณผ ๋น์ฆ๋์ค", url: "/business" },
      { name: "๋น์ฆ๋์ค๋ฅผ ์ํ ์ ํ ์ผํํ๊ธฐ", url: "/retail/business" },
    ],
  },
  {
    title: "๊ต์ก",
    maps: [
      { name: "Apple๊ณผ ๊ต์ก", url: "/education" },
      { name: "์ด์ค๊ณ ์ฉ ์ ํ ์ผํํ๊ธฐ", url: "/education/k12/how-to-buy" },
      {
        name: "๋ํ ์ํ์ ์ํ ์ ํ ์ผํํ๊ธฐ",
        url: "/shop/goto/educationrouting",
      },
    ],
  },
  {
    title: "Apple์ ๊ฐ์น๊ด",
    maps: [
      { name: "์์ฌ์ด ์ฌ์ฉ", url: "/accessibility" },
      { name: "ํ๊ฒฝ", url: "/environment" },
      { name: "๊ฐ์ธ์ ๋ณด ๋ณดํธ", url: "/privacy" },
      { name: "ํ๋ ฅ์์ฒด์ ๋ํ ์ฑ์", url: "/supplier-responsibility" },
    ],
  },
  {
    title: "Apple ์ ๋ณด",
    maps: [
      { name: "Newsroom", url: "/newsroom" },
      { name: "Apple ๋ฆฌ๋์ญ", url: "/leadership" },
      { name: "์ฑ์ฉ ์๋ด", url: "/careers" },
      { name: "์ค๋ฆฌ ๋ฐ ๊ท์  ์ค์", url: "/compliance" },
      { name: "์ด๋ฒคํธ", url: "/apple-events" },
      { name: "์ผ์๋ฆฌ ์ฐฝ์ถ", url: "/job-creation" },
      { name: "Apple ์ฐ๋ฝ์ฒ", url: "/contact" },
    ],
  },
];
```
