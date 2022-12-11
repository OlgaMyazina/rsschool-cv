# Olga Myazina

---
Frontend developer

## Contact

---

- Telegram: @olga_myazina
- Github: olgamyazina
- Discord: olga.myazina

## Profile

---

- Passionate about frontend for 4 years
- Enjoys helping others
- Learning English (endless process)
- tried to [channel](https://dzen.ru/a/YqY1d1shgxK2Q2Ug)

## Stack

---

- React
- Redux + Redux-toolkit
- Lerna
- Microfrontend (Webpack module federation)
- SASS (SCSS)

## Work experience

---

- 2020-2022 Javascript developer in `Company name`
- 2019-2020 Javascript developer freelance

## Education

---

- 2019-2020 SHRI (interface development school)
- 2019 Geekbrains
- 2019 Netology
- 2006-2011 MIREA — RUSSIAN TECHNOLOGICAL UNIVERSITY

## Languages

---

- Russian C1
- English A2-B1

## Code example

---

```javascript

/**
 * @param {number[]} nums
 * @param {number} x
 * @return {number}
 */
const minOperations = (nums, x) => {
  let sum = 0;
  for (let num of nums) {
    sum += num;
  }
  if (sum === x) {
    return nums.length;
  }
  const sumRest = sum - x;
  let maxLength = -1,
    currSum = 0;
  for (let l = 0, r = 0; r < nums.length; r++) {
    currSum += nums[r];
    while (l <= r && currSum > sumRest) {
      currSum -= nums[l++];
    }
    if (currSum === sumRest) {
      maxLength = Math.max(maxLength, r - l + 1);
    }
  }
  return maxLength === -1 ? maxLength : nums.length - maxLength;
};

```




