# Vanya Savickiy

### Contacts:

* Phone: +375 44 731 0906
* e-mail: <isavitskiy8@gmail.com>
* Telegram: @Colnishk0

---

### About me:
Student of the 1st course in the BSU, Minsk on march 2022.

Started learning coding c++ in 10th form. Later it become interesting for me how does the web work.So I started learning html, css and js.

Currently know basics of web, trying to improve my js skills. Want to find people who can share their experience as professional coder, and become a junior programmer in a year or two.

---

### Skills:

* C++
* Wolfram Mathematica
* HTML, Css, JavaScript
* IDE's:
    * VS Code
    * VS
    * Sublime

---

### Code exmaple

Transposition generator for my university's lab

```javascript
let transpositionGen = function(arr)
{
    let returnArr = [];
    let tempArr = arr.slice();

    if(arr.length <= 2)
    {
        let temp = tempArr[0];
        tempArr[0] = tempArr[1];
        tempArr[1] = temp;

        let reverse = tempArr.slice().reverse();
        returnArr.push(reverse);
        returnArr.push(tempArr);

        return returnArr;
    }else
    {
        for(let i = arr.length - 1; i>=0; i--)
        {
            let fixedElem = arr[i];
            tempArr.splice(i, 1);
            let temp = transpositionGen(tempArr);
            
            for(let trans of temp)
            {
                trans.push(fixedElem);
                returnArr.push(trans);
            }
            
            tempArr.splice(i,0,fixedElem);
        }
    }

    return returnArr;
}
```
---

### Job experience

Haven't had, but hope i will get one soon.

---

### Education

* Rsschool (in progress)
* IT-school "Step" (was learning C++ for 1 year)
* University (currently learning web)

---

### English level

Level of English is in the range of B1 INTERMEDIATE to B2 UPPER INTERMEDIATE, according to the guidelines set by the Common European Framework of Reference (CEFR).

