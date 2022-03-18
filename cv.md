# Vanya Savickiy

### Contacts:

* Phone: +375 44 731 0906
* e-mail: <isavitskiy8@gmail.com>
* Telegram: @Colnishk0

### About me:
Student of the 1st course in the BSU, Minsk on march 2022.

Started learning coding c++ in 10th form. Later it become interesting for me how does the web work.So I started learning html, css and js.

Currently know basics of web, trying to improve my js skills. Want to find people who can share their experince as professional coder, and become a junior programmer in a year or two.

### Skills:

* C++
* Wolfram Mathematica
* HTML, Css, JavaScript
* IDE's:
    * VS Code
    * VS
    * Sublime

### Code exmaple:

Transposition generator for my university's lab

```javascript
let transpositionGen = function(arr)
{
    let retrunArr = [];
    let tempArr = arr.slice();

    if(arr.length <= 2)
    {
        let temp = tempArr[0];
        tempArr[0] = tempArr[1];
        tempArr[1] = temp;

        let reverse = tempArr.slice().reverse();
        retrunArr.push(reverse);
        retrunArr.push(tempArr);

        return retrunArr;
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
                retrunArr.push(trans);
            }
            
            tempArr.splice(i,0,fixedElem);
        }
    }

    return retrunArr;
}
```
