# Framework-ready structure

เว็บไซต์ต้นฉบับใช้ HTML/CSS/JavaScript แบบไม่พึ่ง backend เพื่อให้เปิดและ deploy ได้ง่าย

## React / Next.js
- ย้าย section แต่ละส่วนจาก `index.html` เป็น component เช่น `Hero`, `About`, `Experience`, `Skills`, `Education`, `Contact`
- ใช้ `profile-data.json` เป็น data source
- `assets/profile.jpg` และ PDF อยู่ใน `public/assets` และ `public/documents`
- แนะนำ Next.js App Router หากต้องการ SEO และ deploy production

## Vue / Nuxt
- แยก section เป็น Vue components
- import `profile-data.json`
- ย้าย interaction จาก `script.js` ไป composables เช่น `useTheme`, `useScrollReveal`

## PHP / Laravel
- ย้าย HTML เป็น Blade views
- เก็บข้อมูลโปรไฟล์ใน Model/Database ได้ภายหลัง
- assets ไป `public/assets`, documents ไป `public/documents`
- สามารถเพิ่ม Admin CMS เพื่อแก้ไข CV โดยไม่ต้องแก้โค้ด

## Design system
- Primary: deep healthcare green
- Accent: mint/teal
- Typography: IBM Plex Sans Thai + Inter
- Responsive breakpoints: 950px / 620px
- Components are section-based so migration is straightforward
