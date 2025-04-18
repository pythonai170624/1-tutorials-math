# סקלרים וכפל סקלרי במטריצות

## מהו סקלר?

סקלר הוא ערך מספרי בודד בעל גודל אך ללא כיוון. בניגוד לווקטורים או מטריצות (המכילים ערכים מרובים המסודרים במבנים ספציפיים), סקלר הוא פשוט מספר אחד.

### תכונות מרכזיות של סקלרים:
- יכולים להיות מספרים ממשיים (לדוגמה: 5, -3.14, 0)
- יכולים להיות מספרים מרוכבים (לדוגמה: 2+3i)
- משמשים לשינוי קנה מידה של אובייקטים מתמטיים אחרים (וקטורים, מטריצות)
- מיוצגים על ידי משתנים רגילים (לדוגמה: k, c, λ)

### דוגמאות לסקלרים:
- טמפרטורה: 25°C
- מהירות: 60 קמ"ש
- מסה: 5 ק"ג
- זמן: 3 שניות
- מקדמים במשוואות: 2x + 3y = 7 (כאשר 2, 3, ו-7 הם סקלרים)

## דוגמאות לכפל סקלרי

### דוגמה 1: מטריצה 2×2
נתונה מטריצה A:
```
A = [  1   2  ]
    [  3   4  ]
```

כפל סקלרי ב-3:
```
3A = 3 × [  1   2  ] = [  3×1   3×2  ] = [  3   6  ]
         [  3   4  ]   [  3×3   3×4  ]   [  9  12  ]
```

### דוגמה 2: מטריצה 3×3
נתונה מטריצה B:
```
B = [  2   0  -1  ]
    [  4   3   5  ]
    [  1  -2   0  ]
```

כפל סקלרי ב-(-2):
```
-2B = -2 × [  2   0  -1  ] = [ -2×2  -2×0  -2×(-1) ] = [ -4   0   2  ]
           [  4   3   5  ]   [ -2×4  -2×3  -2×5    ]   [ -8  -6 -10  ]
           [  1  -2   0  ]   [ -2×1  -2×(-2) -2×0  ]   [ -2   4   0  ]
```

### דוגמה 3: מטריצות שורה ועמודה
נתונה מטריצת שורה R:
```
R = [  5  -3   0   7  ]
```

כפל סקלרי ב-2:
```
2R = 2 × [  5  -3   0   7  ] = [  2×5  2×(-3)  2×0  2×7  ] = [  10  -6   0  14  ]
```

נתונה מטריצת עמודה C:
```
C = [  2  ]
    [ -1  ]
    [  6  ]
```

כפל סקלרי ב-0.5:
```
0.5C = 0.5 × [  2  ] = [  0.5×2    ] = [  1.0  ]
             [ -1  ]   [  0.5×(-1) ]   [ -0.5  ]
             [  6  ]   [  0.5×6    ]   [  3.0  ]
```

## המחשה ויזואלית

כפל סקלרי במטריצה ניתן להבין כהגדלה או הקטנה של כל הערכים במטריצה באותו יחס. כאשר הסקלר הוא מספר חיובי גדול מ-1, המטריצה "גדלה"; כאשר הסקלר הוא מספר חיובי קטן מ-1, המטריצה "מתכווצת"; וכאשר הסקלר הוא מספר שלילי, המטריצה גם משנה את סימנה.

```
A              x2             Ax2
[  1   2  ]    ---------→     [  2   4  ]
[  3   4  ]                   [  6   8  ]
```

## יישומים של כפל סקלרי

1. **שינוי קנה מידה בגרפיקה ממוחשבת**: שינוי גודל של אובייקטים על ידי הכפלת מטריצות הקואורדינטות שלהם בגורמי קנה מידה.

2. **משוואות בפיזיקה**: המרה בין יחידות (למשל, הכפלת מטריצת מהירות ב-3.6 כדי להמיר ממטר לשנייה לקילומטר לשעה).

3. **מודלים כלכליים**: התאמת מטריצות פיננסיות לאינפלציה או שיעורי צמיחה.

4. **למידת מכונה**: התאמות משקל ברשתות נוירוניות כוללות כפל סקלרי של מטריצות משקל.

5. **עיבוד אותות**: הגברה או החלשה של אותות על ידי הכפלה בגורמי הגבר.

## כפל סקלרי עם מטריצות

כפל סקלרי כולל הכפלה של כל איבר במטריצה בערך סקלרי. ממדי המטריצה נשארים ללא שינוי.

### הגדרה:
אם A היא מטריצה בגודל m×n ו-c הוא סקלר, אז הכפל הסקלרי cA מניב מטריצה בגודל m×n שבה כל איבר של A מוכפל ב-c.

### נוסחה:
עבור מטריצה A = [aᵢⱼ] וסקלר c:
cA = [c × aᵢⱼ]

### תכונות של כפל סקלרי:
1. c(A + B) = cA + cB
2. (c + d)A = cA + dA
3. c(dA) = (cd)A
4. 1A = A
5. 0A = 0 (מטריצת אפסים)
6. (-1)A = -A

# תכונות של מטריצות וכפל סקלרי
## 1. c(A + B) = cA + cB
תכונה זו קובעת שכפל סקלרי של סכום מטריצות שווה לסכום של הסקלר כפול כל מטריצה בנפרד.

### דוגמה:
נגדיר את המטריצות A ו-B:

מטריצה A:
```
A = [1  2]
    [3  4]
```

מטריצה B:
```
B = [5  6]
    [7  8]
```

ונגדיר c = 3

**צד שמאל:** c(A + B)
1. קודם נחשב את A + B:
   ```
   A + B = [1  2] + [5  6] = [6   8]
           [3  4]   [7  8]   [10 12]
   ```
   
2. אז נכפיל ב-c:
   ```
   c(A + B) = 3 × [6   8]  = [18  24]
                  [10 12]    [30  36]
   ```

**צד ימין:** cA + cB
1. קודם נכפיל כל מטריצה ב-c:
   ```
   cA = 3 × [1  2] = [3   6]
            [3  4]   [9  12]
   ```
   
   ```
   cB = 3 × [5  6] = [15  18]
            [7  8]   [21  24]
   ```
   
2. ואז נוסיף את התוצאות:
   ```
   cA + cB = [3   6]  + [15  18] = [18  24]
             [9  12]    [21  24]   [30  36]
   ```

שני הצדדים שווים ל-[18 24; 30 36], ומכאן שהתכונה c(A + B) = cA + cB אכן מתקיימת.

## 2. (c + d)A = cA + dA
תכונה זו קובעת שסכום של סקלרים כפול מטריצה שווה לסכום של כל סקלר כפול המטריצה בנפרד.

### דוגמה:
נגדיר את המטריצה A:

מטריצה A:
```
A = [2  3]
    [4  5]
```

ונגדיר c = 2 ו-d = 3

**צד שמאל:** (c + d)A
1. קודם נחבר את הסקלרים:
   c + d = 2 + 3 = 5
   
2. אז נכפיל את המטריצה בסכום הזה:
   ```
   (c + d)A = 5 ×  [2  3] = [10  15]
                   [4  5]   [20  25]
   ```

**צד ימין:** cA + dA
1. נכפיל את המטריצה בכל סקלר:
   ```
   cA = 2 × [2  3] = [4   6]
            [4  5]   [8  10]
   ```
   
   ```
   dA = 3 × [2  3] = [ 6   9]
            [4  5]   [12  15]
   ```
   
2. ואז נחבר את התוצאות:
   ```
   cA + dA = [4   6]  + [6   9]  = [10  15]
             [8  10]    [12  15]   [20  25]
   ```

שני הצדדים שווים ל-[10 15; 20 25], ומכאן שהתכונה (c + d)A = cA + dA אכן מתקיימת.

## 3. c(dA) = (cd)A
תכונה זו קובעת שכפל של מטריצה בסקלר d ואז בסקלר c שקול לכפל המטריצה במכפלה של שני הסקלרים.

### דוגמה:
נגדיר את המטריצה A:

מטריצה A:
```
A = [1  2]
    [3  4]
```

ונגדיר c = 2 ו-d = 3

**צד שמאל:** c(dA)
1. קודם נכפיל את A ב-d:
   ```
   dA = 3 × [1  2] = [3   6]
            [3  4]   [9  12]
   ```
   
2. ואז נכפיל את התוצאה ב-c:
   ```
   c(dA) = 2 ×  [3   6]  = [ 6  12]
                [9  12]    [18  24]
   ```

**צד ימין:** (cd)A
1. קודם נכפיל את הסקלרים:
   cd = 2 × 3 = 6
   
2. ואז נכפיל את המטריצה במכפלה זו:
   ```
   (cd)A = 6 × [1  2] = [ 6  12]
               [3  4]   [18  24]
   ```

שני הצדדים שווים ל-[6 12; 18 24], ומכאן שהתכונה c(dA) = (cd)A אכן מתקיימת.

## 4. 1A = A
תכונה זו קובעת שכפל מטריצה בסקלר 1 מחזיר את המטריצה המקורית.

### דוגמה:
נגדיר את המטריצה A:

מטריצה A:
```
A = [5  7]
    [2  9]
```

**חישוב:** 1A
```
1A = 1 ×  [5  7] = [5  7]
          [2  9]   [2  9] = A
```

זה מאשר שהתכונה 1A = A אכן מתקיימת.

## 5. 0A = 0 (מטריצת אפסים)
תכונה זו קובעת שכפל של כל מטריצה בסקלר 0 מניב מטריצת אפסים בעלת אותם ממדים.

### דוגמה:
נגדיר את המטריצה A:

מטריצה A:
```
A = [4  8]
    [3  5]
```

**חישוב:** 0A
```
0A = 0 ×  [4  8] = [0  0]
          [3  5]   [0  0]
```

זה מאשר שהתכונה 0A = 0 (מטריצת אפסים) אכן מתקיימת.

## 6. (-1)A = -A
תכונה זו קובעת שכפל מטריצה ב-(-1) שקול להפיכת הסימן של כל איבר במטריצה.

### דוגמה:
נגדיר את המטריצה A:

מטריצה A:
```
A = [2  -3]
    [5   1]
```

**צד שמאל:** (-1)A
```
(-1)A = (-1) ×  [2  -3] = [-2   3]
                [5   1]   [-5  -1]
```

**צד ימין:** -A
```
-A = -[2  -3] =  [-2   3]
      [5   1]    [-5  -1]
```

שני הצדדים שווים ל-[-2 3; -5 -1], ומכאן שהתכונה (-1)A = -A אכן מתקיימת.
