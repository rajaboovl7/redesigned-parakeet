# CSS Box Model & Positioning Practice 📐📍

Ushbu loyiha veb-sahifadagi elementlarning o'lchamlari, ichki va tashqi masofalari (Box Model) hamda ularni sahifa bo'ylab xohlagan joyga joylashtirish (Positioning) qoidalarini amaliyotda o'rganish uchun yaratilgan.

---

## 📦 1. CSS Box Model (Blok Modeli)

Veb-sahifadagi har bir element to'rtburchak quti (box) deb qaraladi. Loyihada ushbu qutining barcha qismlari boshqarilgan:

* **`content`** — Elementning ichidagi matn yoki rasm joylashadigan asosiy qism.
* **`padding`** — Kontent va chegara (border) orasidagi ichki masofa.
* **`border`** — Elementning atrofiga chizilgan chegara.
* **`margin`** — Elementning tashqi tomoni va boshqa elementlar orasidagi masofa.
* **`box-sizing: border-box;`** — Elementning umumiy kengligi va balandligiga `padding` va `border`ni ham hisobga olishni ta'minlaydigan muhim xossa.

---

## 📍 2. CSS Position (Joylashuv xossalari)

Elementlarni sahifada to'g'ri joylashtirish uchun quyidagi `position` turlari amaliyotda qo'llanilgan:

* **`static`** — Standart joylashuv (element kodda qaysi tartibda bo'lsa, shunday ko'rinadi).
* **`relative`** — Element o'zining asl joyiga nisbatan `top`, `right`, `bottom`, `left` xossalari orqali suriladi.
* **`absolute`** — Element o'zidan oldingi `position: relative` (yoki static bo'lmagan) bo'lgan ota-blokiga nisbatan sahifaning istalgan joyiga joylashtiriladi.
* **`fixed`** — Element brauzer oynasiga (ekranga) yopishib qoladi. Sahifa pastga aylantirilganda ham o'z joyidan qimirlamaydi (masalan: Navigatsiya paneli).
* **`sticky`** — Foydalanuvchi sahifani aylantirib, ma'lum bir nuqtaga yetganda element `fixed` kabi qotib qoladi.

---

## 💻 Kodlardan namunalar (Code Snippet)

### Box Model uchun:
```css
.card {
    width: 300px;
    padding: 20px;          /* Ichki masofa */
    border: 2px solid #333; /* Chegara */
    margin: 15px;           /* Tashqi masofa */
    box-sizing: border-box; /* O'lchamni to'g'ri hisoblash */
}
