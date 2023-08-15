Describe: badWordFinder()

Test: "It should return that badWords is an array of our bad words"
Code:
const badWords = ["zoinks", "muppeteer", "biffaroni", "loopdaloop"];
badWords;
Expected Output: ["zoinks", "muppeteer", "biffaroni", "loopdaloop"]

Test: "It should return 1 if a passage has zoinks."
Code:
const text = "zoinks hello";
badWordFinder(text);
Expected Output: 1

Test: "It should return the number of zoinks when calling the first bad word from the badWords array."
Code:
const text = "hello zoinks to zoinks the zoinks";
badWordFinder(text);
Expected Output: 3

Test: "It should return the TOTAL number of zoinks AND the number of muppeteers when calling the first and second words from the badWords array."
Code:
const text = "hello zoinks to zoinks the muppeteer zoinks";
badWordFinder(text);
Expected Output: 3

Test: "It should return the TOTAL number of ALL bad words when calling the individual words from the badWords array."
Code:
const text = "hello zoinks to zoinks the muppeteer zoinks biffaroni, and loopdaloop biffaroni, and loopdaloop";
badWordFinder(text);
Expected Output: 3