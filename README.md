# automation-exe-1-READ ME:

1. הזן :
2. בחר האם 16 או 2 או X :
   • אם בחרת 16- מעביר מהקסדצימלי (בסיס 16) לבינארי
   • אם בחרת 2- נמיר מבינארי להקסדצימלי
   • אם בחרת X: נצא מן המערכת
3. אם הוזן 2:
   a. המערכת תבדוק האם המספר שהוזן תקין (אם יש ערך שונה מאפס או אחד, לא יהיה ניתן להמשיך)
   b. אם המספר תקין- המערכת תבדוק שכמות האיברים מתחלקת ל-4, אם לא, תוסיף אפסים משמאלו עד שיתחלק.
   c. יוגדרו מספר ערכים:
   • BitPos- המיקום בתוך רביעיית איברים
   • StartPos- בודק שעברנו על כל האיברים במספר
   • hexString- המספר ההקסדצימלי שיוחזר
   d. עבור כל מספר ברביעיית איברים:
   • נעלה בחזקת 2 את המיקום שלו ונכפיל בערך שלו
   • נסכום את כל הערכים שקיבלנו
   e. אם הערך שקיבלנו קטן מ-10: נוסיף אותו ל- hexString. אחרת- נמיר אותו לאות בעזרת שימוש בקוד ASCII ורק לאחר מכן נוסיף אותו ל- hexString.
   f. אחרי שעברנו על כל הרביעיות במספר שהוזן- נחזיר hexString
4. אם הוזן 16:
   קודם נמיר מהקסדצימלי לדצימאלי ואח"כ מדצימאלי לבינארי.
   a. המערכת תבדוק האם המספר שהוזן תקין (אם יש ערך שאינו מספר בין 0-9 או אות בין A-F, לא יהיה ניתן להמשיך)
   b. אם המספר תקין נבדוק האם מדובר באות:
   • אם מספר -ישר נמיר לבינארי:
   • נחלק את המספר ב-2 ,נוסיף את השארית שקיבלנו למחרוזת return value ושוב את התוצאה נחלק ב-2 ונוסיף את השארית למחרוזת וכך הלאה עד שהתוצאה אינה מתאפסת.
   • אם אות- נמיר אותה למספר עשרוני באמצעות קוד ASCII (נחסר 55).
   • ואת המספר העשרוני נמיר לבינארי.
   c.
