
# Study Buddy — React Lab

## Note
Follow the **instructions and TODO roadmap in `App.jsx`** carefully.  
All task details, file names, and line references are explained **inside `App.jsx`**.  
Other component files (`CourseCard.jsx`, `TaskItem.jsx`, `DueBadge.jsx`) are intentionally left clean for you to complete.

---

## Overview of the Lab
In this lab, you will build a mini React app called **Study Buddy** — a simple task manager for courses.  
This lab focuses on key React fundamentals you’ve recently studied in ZyBooks.

You will:
- Render course and task lists using `.map()`
- Implement **conditional rendering** using `if`, ternary `? :`, and logical `&&`
- Use **React state (`useState`)** to add, toggle, and delete tasks dynamically

The lab is divided into **four tasks**:
1. Render all courses dynamically (`App.jsx`)
2. Render all tasks inside each course (`CourseCard.jsx`)
3. Add conditional rendering for badges and empty states (`CourseCard.jsx`, `TaskItem.jsx`, `DueBadge.jsx`)
4. Make the app interactive with add, toggle, and delete actions (`CourseCard.jsx`, `TaskItem.jsx`)

---

## Reading Assignment

Before starting, review the following ZyBooks sections:

- [**5.10 Conditional Rendering**](https://learn.zybooks.com/zybook/SWE363Fall2025/chapter/5/section/10)  
- [**5.11 Lists (React)**](https://learn.zybooks.com/zybook/SWE363Fall2025/chapter/5/section/11)

These sections explain the key concepts used in this lab.

---

## Concepts Used in This Lab

### 1. Conditional Rendering
Render UI elements based on conditions using **if**, **ternary**, or **logical AND (`&&`)**.

#### Syntax:
```jsx
// Using if
if (condition) {
  return <ComponentA />;
} else {
  return <ComponentB />;
}

// Using ternary operator
{ condition ? <ComponentA /> : <ComponentB /> }

// Using logical AND
{ condition && <ComponentA /> }
```

---

### 2. Rendering Lists with `.map()`
Generate dynamic components by mapping through an array.

#### Syntax:
```jsx
{array.map((item, index) => (
  <Component key={item.id} prop={item.value} />
))}
```

---

### 3. React Keys
Keys help React identify which items have changed or moved in a list.

#### Syntax:
```jsx
<Component key={uniqueId} />
```

---

### 4. React State (`useState`)
Use state to store and update component data.

#### Syntax:
```jsx
import { useState } from "react";

const [stateVariable, setStateVariable] = useState(initialValue);
```

---

### 5. Event Handling
React events handle user interactions such as clicks and input changes.

#### Syntax:
```jsx
<button onClick={handleClick}>Click Me</button>

<input
  value={value}
  onChange={e => setValue(e.target.value)}
/>
```

---

### 6. Passing Props
Props allow parent components to send data and functions to children.

#### Syntax:
```jsx
<ChildComponent propName={data} anotherProp={functionName} />
```

---

## ✅ Submission Checklist

Before submitting your lab, make sure you have completed and verified each step below:

- [ ] **Task 1:** Course cards are rendered dynamically using `.map()` in `App.jsx`
- [ ] **Task 2:** Tasks are rendered dynamically inside each course using `.map()` in `CourseCard.jsx`
- [ ] **Task 3:** Conditional rendering is working (badges, empty states, due dates)
- [ ] **Task 4:** Adding, toggling, and deleting tasks work correctly
- [ ] **Code style:** Proper indentation, meaningful variable names
- [ ] **No console errors** when running the app
- [ ] **Optional:** Add creative touches (colors, labels, emoji, etc.)

---

