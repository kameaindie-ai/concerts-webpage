# אתר הופעות קמע — הוראות העלאה ל-GitHub Pages

הקובץ `index.html` הוא כל האתר (HTML+CSS+SVG בקובץ אחד, אין תלות בקבצים חיצוניים חוץ מפונטים מ-Google Fonts).

## שלבי העלאה

1. ליצור ריפו חדש ב-GitHub (Public — חובה לגרסה החינמית של Pages).
2. להעלות את `index.html` לשורש הריפו (root), בדיוק בשם הזה — `index.html`.
3. ב-GitHub: **Settings → Pages**
   - Source: **Deploy from a branch**
   - Branch: **main** (או master) **/ (root)**
   - Save.
4. אחרי דקה-שתיים האתר יהיה זמין בכתובת:
   `https://<username>.github.io/<repo-name>/`

## חיבור דומיין מותאם אישית (shows.kameamusic.co.il)

1. באותו מסך **Settings → Pages**, בשדה **Custom domain** להזין `shows.kameamusic.co.il` ולשמור — GitHub ייצור אוטומטית קובץ `CNAME` בריפו.
2. אצל ספק הדומיין (Wix) להוסיף רשומת **CNAME**:
   - Host/Name: `shows`
   - Value/Target: `<username>.github.io`
3. להמתין להתעדכנות DNS (עד יממה).
4. מומלץ לסמן גם **Enforce HTTPS** בהגדרות ה-Pages לאחר שהדומיין מאומת.

## עדכון תוכן בהמשך

כל עדכון (הופעה חדשה, שינוי טקסט) הוא פשוט עריכת `index.html` והעלאה מחדש (commit + push) לאותו ריפו — האתר מתעדכן אוטומטית תוך דקה, בלי שום צעד נוסף.
