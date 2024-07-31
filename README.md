# Javascript_Coding_Questions
## Next Vowel Replacement

### Description

Write a function that takes an input string and replaces each vowel with the next vowel in the sequence `a -> e -> i -> o -> u -> a`. 

For example, given the input string "Palak", the output should be "Pelek".

### Input

- A single string `input` consisting of lowercase and uppercase alphabets.

### Output

- A single string where each vowel in the input string is replaced with the next vowel.

### Example

```
const replaceChar = {
    'a': 'e',
    'e': 'i',
    'i': 'o',
    'o': 'u',
    'u': 'a',
    'A': 'E',
    'E': 'I',
    'I': 'O',
    'O': 'U',
    'U': 'A'
};

function nextVowelReplacement(input) {
    let result = "";
    for (let char of input) {
        if (replaceChar[char]) {
            result += replaceChar[char];
        } else {
            result += char;
        }
    }
    return result;
}

let input = "Palak";
console.log(nextVowelReplacement(input));  // Output: "Pelek"
'''
