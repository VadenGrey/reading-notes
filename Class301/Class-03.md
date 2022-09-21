# Class 03

**React docs**
1. an array
2. 

```

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

```

3. key
4. keys help identitfy items


**Spread Operator**
1. syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
2. Concatenating or combining arrays, Using an array as arguments, Combining objects, Converting NodeList to an array
3. 

```

const y = [1,2,3,4];
const x = [5,6,7,8];
const z = [...x,...y];
console.log(z)

```

4. 

```

const y = [1,2,3,4];
const x = 5;
const z = [...x,...y];
console.log(z)

```

5. 

```

const y = {name: 'y'};
const x = {name: 'y'};
const z = {...x,...y};
console.log(z)

```

**pass functions between componenets**
1. make the function inside an object
2. increments the value 'count' in each object selected
3. by referencing the function within the child with 'this.function'
4. using props

**things I want to know more about**

references

[React docs](https://reactjs.org/docs/lists-and-keys.html)

[Spread Operator](https://www.youtube.com/watch?v=IYvD9oBCuJI&ab_channel=WebDevSimplified)

[pass functions between componenets](https://www.youtube.com/watch?v=c05OL7XbwXU&ab_channel=SteveGriffith-Prof3ssorSt3v3)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)
