# 🇮🇷 @snapp-store/iranian-banks-react-icons

A comprehensive collection of **React icons** for Iranian banks, PSPs, and financial institutions.  
Includes both **colored** and **monotone** SVG variants for each logo — ready to use in React or React Native (with SVG support).

---

## 🏦 Supported Brands

This package includes icons for almost all Iranian banks and payment providers, such as:

- Bank Melli, Mellat, Saderat, Tejarat, Sepah, Pasargad, Saman, Refah, Keshavarzi, Maskan, etc.  
- Newer banks: BluBank, Bankino, Futurebank, Iran Zamin, Ayandeh, Melall, Sarmayeh, etc.  
- PSPs and fintechs: Zarrinpal, Pay.ir, Payping, NextPay, IdPay, Vandar, SnappPay, Digipay, etc.  
- Payment networks and institutions: Shaparak, Bank Markazi, Iran Europe, Standard Chartered, and more.

Each brand includes two variants:
- **ColorIcon** → full-color version of the official logo  
- **Icon** → monochrome (solid) version

---

## 📦 Installation

```bash
# with npm
npm install @snapp-store/iranian-banks-react-icons

# or with yarn
yarn add @snapp-store/iranian-banks-react-icons
```

---

## 🚀 Usage

Each icon is exported as a named ES module.

### Example

```jsx
import {
  MelliColorIcon,
  MelliIcon,
  PasargadColorIcon,
  ZarrinpalIcon
} from '@snapp-store/iranian-banks-react-icons';

export default function Example() {
  return (
    <div style={{ display: 'flex', gap: 16, alignItems: 'center' }}>
      <MelliColorIcon width={48} height={48} />
      <MelliIcon width={48} height={48} fill="#333" />
      <PasargadColorIcon width={48} height={48} />
      <ZarrinpalIcon width={48} height={48} fill="#000" />
    </div>
  );
}
```

All icons are **React components** that accept standard SVG props:
```tsx
type IconProps = React.SVGProps<SVGSVGElement>;
```

---

## 🧱 CommonJS Support

You can also import using `require` (Node-style):

```js
const { MelliIcon, MellatColorIcon } = require('@snapp-store/iranian-banks-react-icons');
```

Each export maps directly to an individual `.js` file, for example:

```js
module.exports.MelliIcon = require('./MelliIcon.js');
module.exports.MelliColorIcon = require('./MelliColorIcon.js');
```

---

## 🖌️ Naming Convention

Each icon follows this consistent naming pattern:

| Type | Example | Description |
|------|----------|-------------|
| Color version | `MelliColorIcon` | Official multicolor SVG |
| Monochrome version | `MelliIcon` | Single-color (solid) variant |

---

## ⚙️ Tech Details

- ✅ Framework: React (no dependencies other than `react` and `react-dom`)
- ✅ File format: optimized inline SVG components
- ✅ Supports tree-shaking — import only what you need
- ✅ Compatible with TypeScript

---

## 🧩 List of Available Icons

<details>
<summary>Click to expand</summary>

```
AsanPardakht, Ayandeh, BankMarkazi, Bankino, BluBank, Caspian, Dey, Digipay,
EghtesadNovin, Futurebank, Gardeshgari, Hesabit, Idpay, IranEurope, IranVenezuela,
IranZamin, Karafarin, Keshavarzi, KhavarMianeh, Maskan, MehrIran, Melall, Mellat,
Melli, NextPay, Noor, Parsian, Pasargad, PasargadPep, PayIr, Payping, Post, Refah,
Resalat, Sadad, Saderat, Saman, SamanKish, SanatMadan, Sarmayeh, Sepah, SepahMerged*,
Shahr, Shaparak, Sina, SnappPay, StandardChartered, TaavonEslami, Tejarat, Tosee,
ToseeSaderat, ToseeTaavon, Vandar, Zarrinpal, Zibal
```

Each with both `Icon` and `ColorIcon` variants.
</details>

---

## 🧠 Example with Dynamic Rendering

You can dynamically render a logo by name:

```jsx
import * as Icons from '@snapp-store/iranian-banks-react-icons';

function BankLogo({ name }) {
  const Icon = Icons[`${name}ColorIcon`] || Icons[`${name}Icon`];
  return Icon ? <Icon width={48} height={48} /> : null;
}

<BankLogo name="Saderat" />;
```

---

## 📄 License

MIT © Snapp Store  
Feel free to use and modify in your React projects.

---

## 💬 Contributing

Pull requests and new icons are welcome!  
If you find missing or outdated logos, open an issue or PR on [GitHub](https://github.com/snapp-store/iranian-banks-react-icons).
