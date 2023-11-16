# Palindrome

<h2>Exercise</h2>
<p>Return true if the given string is a palindrome. Otherwise, return false.</p>
<p>A palindrome is a word or sentence that's spelled the same way both forward and backward, ignoring punctuation, case, and spacing.</p>
<p>Note: You'll need to remove all non-alphanumeric characters (punctuation, spaces and symbols) and turn everything into the same case (lower or upper case) in order to check for palindromes.</p>
<p>We'll pass strings with varying formats, such as racecar, RaceCar, and race CAR among others.</p>
<p>We'll also pass strings with special symbols, such as 2A3*3a2, 2A3 3a2, and 2_A3*3#A2.</p>

<h2>Code</h2>

```
function palindrome(str) {
  const strN = str.replace(/[^a-zA-Z0-9]/g, '').toLowerCase();
  let reps = strN === strN.split('').reverse().join('')
  return console.log('==================\nPalindrome Checker\n==================\nWord: '+str+'\nReverse: '+strN+'\nResult: '+reps);
}
```

<h2>Exemple</h2>

```
palindrome("eye");

==================
Palindrome Checker
==================
Word: eye
Reverse: eye
Result: true
```
<a href="https://a-marvulle.github.io/palindrome/" target=_blank>Pages</a>
