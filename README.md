# Convert English To Nepali Number


```js

function convertEnglishNumberToNepaliNumber(value){
  if (value === null || value === undefined) {
    return 0;
  }
  const numbersInNepali = {
    0: "०",
    1: "१",
    2: "२",
    3: "३",
    4: "४",
    5: "५",
    6: "६",
    7: "७",
    8: "८",
    9: "९"
  };
  const valueToString = value.toString();
  const arrayValue = valueToString.split("");
  const normalizeArrayValue = arrayValue.map(value => {
    return numbersInNepali[value];
  });
  return normalizeArrayValue.join("");
};

convertEnglishNumberToNepaliNumber(120)   // १२०
convertEnglishNumberToNepaliNumber(1234)   // १२३४

```
