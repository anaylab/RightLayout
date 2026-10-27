[English](README.md) | [Русский](README.ru.md) | [עברית](README.he.md)

<div align="center" dir="rtl">

# RightLayout

**הקלידו בחופשיות.**

RightLayout מתקן טעויות במקלדת עוד לפני שהבחנתם בהן.

[הורדה ל-Mac](https://github.com/chernistry/RightLayout/releases/latest) · [אתר](https://alexchernysh.com/rightlayout)

---

*[English](README.md) · [Русский](README.ru.md) · [עברית](README.he.md)*

*macOS 13+ · חינמי · קוד פתוח*

</div>

---

<div dir="rtl">

> **הפרויקט מתוחזק כעת על ידי הקהילה. היוצר המקורי אינו מפתח אותו באופן פעיל. תרומות יתקבלו בברכה!**

</div>

---

<div dir="rtl">

## איך זה עובד

אתם מקלידים בפריסת מקלדת שגויה, ו-RightLayout מתקן את הטקסט מיד באמצעות בינה מלאכותית שרצה על המכשיר עצמו (CoreML).

</div>

```
ghbdtn  →  привет
руддщ   →  hello  
akuo    →  שלום
```

<div dir="rtl">

בלי קיצורי מקשים. בלי התראות. רק טקסט נכון.

</div>

---

<div dir="rtl">

## יכולות

**עובד בלי להפריע**  
בלי חלונות קופצים ובלי הפרעות. התיקונים מתבצעים תוך כדי הקלדה.

**זיהוי שפה מבוסס בינה מלאכותית**  
מודל CoreML שאומן על נתוני הקלדה אמיתיים במגוון שפות מזהה טקסט שהוקלד בפריסה שגויה ברמת דיוק גבוהה.

**לומד אתכם**  
ביטלתם תיקון פעמיים? RightLayout זוכר. הוא מתאים את עצמו לסגנון הכתיבה שלכם.

**שומר על הפרטיות**  
הכול רץ על ה-Mac שלכם. שום דבר לא עוזב את המכשיר. אף פעם.

**תמיכה במקלדות בכמה שפות**  
תומך בפריסות באנגלית, ברוסית ובעברית, עם ארכיטקטורה שמאפשרת להוסיף שפות נוספות.

</div>

---

<div dir="rtl">

## התקנה

1. הורידו את קובץ ה-`.pkg` מעמוד ה-[Releases](https://github.com/chernistry/RightLayout/releases/latest)
2. הפעילו את תוכנית ההתקנה
3. אשרו הרשאת נגישות (Accessibility) כשתתבקשו
4. זהו. RightLayout פועל ברקע

</div>

---

<div dir="rtl">

## בנייה מקוד המקור

</div>

```bash
git clone https://github.com/chernistry/RightLayout.git
cd RightLayout
swift build
swift test
```

<div dir="rtl">

נדרשים macOS 13+‎, Xcode 15+‎ ו-Swift 5.10+‎.

להנחיות על הגדרת סביבת הפיתוח, סגנון הקוד והוספת שפות חדשות, ראו את [CONTRIBUTING.md](CONTRIBUTING.md).

</div>

---

<div dir="rtl">

## מחפשים מתחזקים

הפרויקט זקוק למתחזקים חדשים. אם יש לכם עניין בפיתוח ל-macOS, בטיפול בקלט מהמקלדת או בזיהוי שפה מבוסס CoreML, זה פרויקט מצוין לקחת תחת חסותכם.

**מה עושה מתחזק:**
- ממיין ועונה על Issues
- בודק ומאשר Pull Requests
- מפיץ גרסאות חדשות
- מרחיב את התמיכה בשפות (גרמנית, צרפתית, ערבית ועוד)

אם זה מעניין אתכם, פתחו Issue בשם "Maintainer interest" וספרו על הרקע שלכם. אין שומרי סף: מי שמגיש PRs טובים מקבל הרשאות כתיבה.

</div>

---

<div dir="rtl">

## ארכיטקטורה

</div>

- `RightLayout/Sources/Engine/` — ליבת התיקון (זיהוי שפה, מיפוי פריסות, ניתוב לפי רמת ביטחון)
- `RightLayout/Sources/UI/` — הגדרות ב-SwiftUI וממשק בשורת התפריטים
- `RightLayout/Sources/Settings/` — העדפות משתמש והתאמה אישית
- `Tools/CoreMLTrainer/` — צינור האימון ב-Python של מסווג השפה ל-CoreML

<div dir="rtl">

פרטים על הוספת יכולות ושפות מופיעים ב-[CONTRIBUTING.md](CONTRIBUTING.md).

</div>

---

<div dir="rtl">

## רישיון

Apache-2.0 — ראו [LICENSE](LICENSE). השימוש בשם הפרויקט: [TRADEMARKS.md](TRADEMARKS.md).

</div>

---

<div align="center" dir="rtl">

נוצר על ידי [Alex Chernysh](https://alexchernysh.com)

</div>

<div dir="rtl">

התרגום מבוסס על [README.md מהקומיט a80820807643118ac24144d5da6b06de2b1a4d70](https://github.com/chernistry/RightLayout/blob/a80820807643118ac24144d5da6b06de2b1a4d70/README.md).

</div>
