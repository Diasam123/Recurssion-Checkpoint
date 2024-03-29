function isPalindrome(word) {
  // Check the stop condition
  if (word.length <= 1) {
    return true;
  }

  // Compare characters at the ends of the word
  if (word[0] === word[word.length - 1]) {
    // Recursively test the rest of the word
    return isPalindrome(word.slice(1, -1));
  } else {
    return false;
  }
}

// Example usage:
const words = ["gag", "kayak", "php", "radar", "openai", "javascript"];
for (const word of words) {
  if (isPalindrome(word)) {
    console.log(`${word} is a palindrome.`);
  } else {
    console.log(`${word} is not a palindrome.`);
  }
}

In this JavaScript implementation, the isPalindrome function follows the same logic. It checks the stop condition for an empty word or a word with a length of 1. If the word has more than one character, it compares the first and last characters. If they are equal, it recursively tests the rest of the word using slice to exclude the first and last characters. If the characters are different, it returns false since the word is not a palindrome.

The example usage demonstrates how to test multiple words using the isPalindrome function. It logs whether each word is a palindrome or not using console.log.#   R e c u r s s i o n - C h e c k p o i n t  
 