## **[rsschool-cv](https://KissMyUSSR.github.io/rsschool-cv/cv)**

# **Kirill Cherepanov**

## **Contacts**

* **Location: Belarus, Minsk**
* **Email: cherkirr@gmail.com**
* **GitHub: @KissMyUSSR**
* **VK: https://vk.com/kcherepanov1**
* **Discord: Kot-pauk#6737**

## **About me** 
I used to play a lot of video games for the entirety of my life, but one horrible day I realized that my PC sucks and I can no longer play my games. Thus I strongly decided to become a web developer to earn some money for a living and for a new PC to proceed with my beloved lifestyle.

Just joking. I'm a reliable person and I love helping others. One may even call me altruistic, though I am not willing to help others when it might hurt myself. I love learning new stuff and new technologies. And if I like doing something, I may spend 16 hours a day doing it (if I have all this time). Also, I'm quite good at Math and it comes easily for me. Also I have a nice English level, but later on that.

## **My skills**
* HTML5, CSS3
* Javascript basics
* Python, Most of the standart library
* VS Code, PyCharm
* Git
* Playing games & binge-watching anime

## **Code example**
### [Sudoku Solution Validator](https://www.codewars.com/kata/529bf0e9bdf7657179000008/javascript)
```
// It's mildly inafficient but idc for now.

function sliceColumn(mat, index) {
  let column = [];
  for (let i = 0; i < mat.length; i++) {
    column.push(mat[i][index]);
  }
  return column;
}
function validSolution(board) {
  let checkArr = [];
  for (let i = 0; i < 9; i++) {
    for (let j = 0; j < 9; j++) {
      if ((board[i].slice(0, j) + board[i].slice(j + 1, 9)).includes(board[i][j])) return false;
      if ((sliceColumn(board, i).slice(0, j) + sliceColumn(board, i).slice(j + 1, 9)).includes(board[j][i])) return false;
    }
  }
  for (let i = 0; i < 7; i+=3) {
    for (let j = 0; j < 7; j+=3) {
      for(let t = 0; t < 9; t++) {
        if ( checkArr.includes(board[i + t % 3][j + (t - t % 3)/3]) ) return false;
        checkArr.push(board[i + t % 3][j + (t - t % 3)/3]);
      }
      checkArr = [];
    }
  }
  
  return true;
}
```

## **Education**
* Mechanics and Mathematics Faculty of BSU, 2nd course
* [The Web Developer Bootcamp](https://www.udemy.com/course/the-web-developer-bootcamp/)
* *And youtube lectures which I can't remember*

## **Languages**
* **English** - I'm quite profficient at it and the online tests that I participated in showed that I have an advanced C1-C2 level. Though I don't trust these tests much and I've never taken any reliable tests e.g. IELTS or something.
[![One of the test results](/images/My%20eng%20level.jpg)](https://www.facebook.com/permalink.php?story_fbid=3024079811203680&id=100008050725980)
* **Russian** - Native.
* **Japanese** - the very basics, but I'd really like to learn it if I had enough time.
* **Belarussian** - though I'm Belarussian, I know Japanese better than this one.