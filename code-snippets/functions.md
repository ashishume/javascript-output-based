<div align="center">
  <h1>Functions</h1>
</div>

<ol>

<li>

**What will be the Output??**

```JS
function setName() {
   this.name = 'devkode';
}

setName();
console.log(this.name);
```

- A: `‘devkode’`
- B: `undefined`
- C: `An Error will be thrown`
- D: `null`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>

</li>

---

<li>

**What will be the output ?**

```JS
function fun(num1) {
    var num2 = 6;

    function TDK() {
        var num3 = 10;
        console.log(num1 * num2 * num3)
    }

    return TDK;
}

var TeamDevKode = fun(5)
TeamDevKode ()
```

- A: `undefined`
- B: `0`
- C: `300`
- D: `infinity`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>

</li>

---

<li>

**What is the output ?**

```JS
const animal = {
  animal_name: "cat",
  action: function () {
    console.log(`${this.animal_name} is doing action`);
  }
};

setTimeout(animal.action, 1000);

```

- A: `cat is doing action`
- B: `undefined is doing action`
- C: `null is doing action`
- D: `error`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: B

</p>
</details>

</li>

---

<li>

**What is the output ?**

```JS
const animal = {
  animal_name: "cat",
  action: function () {
    console.log(`${this.animal_name} is doing action`);
  }
};

setTimeout(function () {
  animal.action();
}, 1000);

```

- A: `cat is doing action`
- B: `undefined is doing action`
- C: `null is doing action`
- D: `error`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>

</li>

---

<li>

**What is the output ?**

```JS
const animal = {
  animal_name: "cat",
  action: function () {
    console.log(`${this.animal_name} is doing action`);
  }
};

let func = animal.action.bind(animal);
setTimeout(func, 1000);

```

- A: `null is doing action`
- B: `undefined is doing action`
- C: `cat is doing action`
- D: `error`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>

</li>

---

<li>

**What is the output ?**

```JS
function getFunc() {
  let value = "Hey !";

  let func = new Function("console.log(value)");

  return func;
}

getFunc()();

```

- A: `Hey !`
- B: `error: value is not defined`
- C: `null`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: B

</p>
</details>

</li>

---

<li>

**What is the output ?**

```JS
function getFunc() {
  let value = "Hello Friends !";
  let func = () => {
    alert(value);
  };
  return func;
}

getFunc()();

```

- A: `Hey !`
- B: `error: value is not defined`
- C: `Hello Friends !`
- D: `null`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>

</li>

---

</ol>