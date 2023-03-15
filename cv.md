# Maria Regnard

## Junior React Developer

## Contacts:

**Email**: alece.1414@gmail.com

# **Telegram**: @malfrav

## About me:

Passionate frontend developer. My main tech-stack is React + Redux, but I'm always interested in other technologies.

## Skills:

- React
- Redux
- Javascript ES6
- HTML5
- CSS3
- SASS
- Git
- Responsive design
- REST API

## Code example:

Given n points on a 2D plane, find if there is such a line parallel to y-axis that reflect the given points.

Example 1: Given points = [[1,1],[-1,1]], return true.

Example 2: Given points = [[1,1],[-1,-1]], return false.

```
const reflectDotes = (dotes) => {
  let xmin = dotes[0][0];
  let xmax = dotes[0][0];

  const coordinates = {};

  for (let i = 0; i < dotes.length; i++) {
    const x = dotes[i][0];
    const y = dotes[i][1];

    xmin = Math.min(xmin, x);
    xmax = Math.max(xmax, x);

    if (coordinates[y]) {
      coordinates[y].push(x);
    } else {
      coordinates[y] = [];
      coordinates[y].push(x);
    }
  }

  const middle = (xmax + xmin) / 2;
  const doublebar = xmax + xmin;

  for (let i = 0; i < dotes.length; i++) {
    const x = dotes[i][0];
    const y = dotes[i][1];

    const mx = doublebar - x;
    if (!coordinates[y].includes(mx) && y !== middle) {
      return false;
    }
  }

  return true;
};
```

## Courses:

- JAVASCRIPT + REACT COURSE BY IVAN PETRICHENKO, Udemy (completed)
- WEB-DEVELOPER BY IVAN PETRICHENKO, Udemy (completed)
- RS Schools Course «JavaScript/Front-end. Stage 1» (in progress)

## Languages:

- Russian - Native
- English - C1
- Italian - B2
