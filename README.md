# Js-DOM.p---Cube

<img width="1726" height="818" alt="image" src="https://github.com/user-attachments/assets/a08915a5-09d1-48d7-8160-a2898fa372de" />

להלן **מדריך לימודי מוכן ל-GitHub (README.md)** שמסביר **מה לומדים ב-JavaScript** דרך הפרויקט ששלחת 👇
המדריך מותאם ללמידה, להצגה בתיק עבודות, ולהבנה הדרגתית של JS דרך פרויקט ויזואלי.

---

# 🎲 3D Cube Slider – JavaScript Learning Guide

פרויקט זה מדגים כיצד להשתמש ב־**JavaScript** כדי לשלוט באלמנטים תלת־ממדיים ב־CSS, לנהל מצב (state), לעבוד עם אירועים, ולבנות לוגיקה אינטראקטיבית מלאה.

---

## 🎯 מטרות לימוד

בפרויקט זה נלמד:

* איך JavaScript שולט ב־HTML ו־CSS
* איך יוצרים אינטראקציה עם המשתמש
* איך עובדים עם משתנים, פונקציות וטיימרים
* איך מנהלים מצב של אפליקציה (State)
* איך יוצרים אנימציות לוגיות (לא רק CSS)

---

## 🧠 נושאים עיקריים ב-JavaScript שנלמדים בפרויקט

---

### 1️⃣ משתנים ו־State (מצב מערכת)

```js
let x = 0, bool = false, interval;
```

🔹 מה לומדים כאן:

* `x` – שומר את זווית הסיבוב של הקובייה
* `bool` – בודק האם האנימציה פועלת (play / pause)
* `interval` – שומר טיימר להפעלה/עצירה

📌 זהו **State** – מידע שמשפיע על התנהגות האפליקציה.

---

### 2️⃣ בחירת אלמנטים מה־DOM

```js
document.querySelector('.left-arrow')
document.querySelectorAll('.cube')
```

🔹 מה לומדים כאן:

* גישה לאלמנטים ב־HTML
* עבודה עם מחלקות (`class`)
* שליטה על כמה אלמנטים יחד (`querySelectorAll`)

---

### 3️⃣ פונקציות (Functions)

```js
const rotate = () => {
  const cubes = document.querySelectorAll('.cube');
  cubes.forEach(cube => {
    cube.style.transform = `rotateY(${x}deg)`;
  });
}
```

🔹 מה לומדים כאן:

* יצירת פונקציה
* שימוש ב־Arrow Functions
* שינוי CSS דרך JavaScript
* הפרדת לוגיקה לפונקציות קריאות וברורות

---

### 4️⃣ עבודה עם CSS דרך JavaScript

```js
cube.style.transform = `rotateY(${x}deg)`
```

🔹 מה לומדים כאן:

* שינוי עיצוב דינמי
* חיבור בין JS ל־CSS 3D
* שליטה באנימציות דרך לוגיקה

---

### 5️⃣ Event Listeners – תגובה לפעולות משתמש

```js
element.addEventListener('click', () => {})
element.addEventListener('mouseover', () => {})
element.addEventListener('mouseout', () => {})
```

🔹 מה לומדים כאן:

* האזנה לאירועים
* יצירת חוויית משתמש אינטראקטיבית
* הבדל בין `click`, `hover`, `leave`

---

### 6️⃣ עבודה עם לולאות (Loops)

```js
Array.from(cubes).forEach(cube => { ... })
```

🔹 מה לומדים כאן:

* מעבר על אוסף אלמנטים
* שימוש ב־`forEach`
* כתיבה מודרנית ונקייה

---

### 7️⃣ טיימרים – setInterval / clearInterval

```js
interval = setInterval(() => {
  x -= 90;
  rotate();
}, 1000);
```

🔹 מה לומדים כאן:

* אנימציה מבוססת זמן
* הפעלה והפסקה של תהליך
* שליטה בקצב (timing)

---

### 8️⃣ שינוי מחלקות (Class Manipulation)

```js
i.classList.add('fa-pause');
i.classList.remove('fa-play');
```

🔹 מה לומדים כאן:

* שינוי אייקונים דינמית
* עבודה עם `classList`
* חיבור ל־UI (Font Awesome)

---

### 9️⃣ לוגיקה ותנאים (if / else)

```js
if (!bool) {
  play();
} else {
  pause();
}
```

🔹 מה לומדים כאן:

* קבלת החלטות
* ניהול מצבים
* מניעת התנגשויות לוגיות

---

## 🚀 למה הפרויקט הזה מצוין ללמידה?

✔ פרויקט ויזואלי – רואים תוצאה מיידית
✔ משלב JS + CSS + HTML
✔ מדמה לוגיקה של אפליקציה אמיתית
✔ מתאים למעבר ל־React / Next.js
✔ מצוין לתיק עבודות

---

## 📌 למי הפרויקט מתאים?

* תלמידים מתחילים ב־JavaScript
* מפתחי Frontend בתחילת הדרך
* מורים לתכנות
* מי שרוצה להבין **איך JS באמת עובד**

---👍


