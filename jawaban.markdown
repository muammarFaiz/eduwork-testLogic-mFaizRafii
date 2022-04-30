1. edit integer
    
    ```js
      function editInt(theInt) {
        let i = 0, output = 1
        while (i < theInt - 1) {
          output = output * (theInt - i)
          i++
        }
        console.log(output);
      }
    ```

2. reverse string

    ```js
      function editStr(theStr) {
        let i = 0, result = ''
        while (i < theStr.length) {
          result = result + theStr[theStr.length - (i + 1)]
          i++
        }
        console.log(result);
      }
    ```

3. printDigitValue

    ```js
    function printDigitValue(theStr) {
      let i = 0, theNum = ''
      while (i < theStr.length) {
        if(parseInt(theStr[i], 10)) {
          theNum = theNum + theStr[i]
        }
        i++
      }
      console.log(parseInt(theNum, 10));
      let i2 = 0, tolog = ''
      while(i2 < theNum.length) {
        const amount = (theNum.length - 1) - i2
        let i3 = 0, zeros = ''
        while(i3 < amount) {
          zeros = zeros + '0'
          i3++
        }
        console.log(theNum[i2] + zeros);
        i2++
      }
    }
    ```

4. swap variables

    ```js
      let a = 5;
      let b = 7;
      [a, b] = [b, a];
      console.log(a, b);
    ```

5. naming number

    ```js
      function x (n) {
        function thestring(int) {
          switch (int) {
            case 0:
              return 'nol'
            case 1:
              return 'satu'
            case 2:
              return 'dua'
            case 3:
              return 'tiga'
            case 4:
              return 'empat'
            case 5:
              return 'lima'
            case 6:
              return 'enam'
            case 7:
              return 'tujuh'
            case 8:
              return 'delapan'
            case 9:
              return 'sembilan'
            default:
              break;
          }
        }

        let front = parseInt(n.toString()[0], 10)
        if (n > 9) {
          let back = parseInt(n.toString()[1], 10)
          if(n > 10 && n < 20) {
            if(n === 11) {
              console.log('sebelas');
            } else {
              console.log(thestring(back) + ' belas')
            }
          } else if(n === 100) {
            console.log('seratus');
          } else if(n < 101) {
            if (n === 10) {
              console.log('sepuluh');
            } else if(back) {
              console.log(thestring(front) + ' puluh ' + thestring(back));
            } else {
              console.log(thestring(front) + ' puluh');
            }
          } else {
            console.log('silahkan masukkan bilangan 1-100');
          }
        } else if(n < 0) {
          console.log('silahkan masukkan bilangan 1-100');
        } else {
          console.log(thestring(front));
        }
    ```

6. filter array

    ```js
    function filterArr(arr, low, high) {
      const newArr = arr.filter(int => {
        if(int > low && int < high) {
          return true
        }
      })
      console.log(newArr);
    }
    ```

7. total filter array

    ```js
    function filterArr(arr, low, high) {
      const newArr = arr.filter(int => {
        if(int > low && int < high) {
          return true
        }
      })
      console.log(newArr.length);
    }
    ```

8. tiga dan lima

    ```js
    function trif(int) {
      let i = 1
      while(i <= int) {
        if(i%3 === 0 && i%5 === 0) {
          console.log('eduwork');
        } else if(i%3 === 0) {
          console.log('edu');
        } else if(i%5 === 0) {
          console.log('work');
        } else {
          console.log(i);
        }
        i++
      }
    }
    ```

# oh oh waktu habis