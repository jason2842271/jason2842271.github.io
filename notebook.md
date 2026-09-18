## Table of Contents
- [Blocks](#blocks)
- [Concepts](#concepts)
- [Vocabulary](#vocabulary)
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)
  - [Headings](#headings)
  - [Text Formatting](#text-formatting)

## Blocks

Each VEXcode VR program should begin with a **starter block**, usually the hat-shaped block. The blocks below explain the shape, purpose, and use of each block.

### Hat Block

- **Shape/Type:** Hat-shaped starter block.
- **What it does:** Starts the program. Blocks connected below it run when the program begins.
- **Example:** Put the hat block at the top, then connect `drive forward` below it.

### Stack / Command Block

- **Shape/Type:** Rectangular stack block.
- **What it does:** Performs an action, such as driving, turning, or moving a pen.
- **How it connects:** Stack blocks connect above and below one another to form a sequence of commands. Some command blocks can also hold other blocks in their input slots.
- **Example:** Connect `drive forward` after the starter block to make the VR Robot move.

### C-Block

- **Shape/Type:** C-shaped control block.
- **What it does:** Holds other blocks and controls when or how often those blocks run.
- **Why blocks fit inside:** The open space acts like a container for instructions used by a loop or conditional.
- **Example:** Place `turn right` inside a `repeat` block to turn several times.

### Reporter / Oval Block

- **Shape/Type:** Oval-shaped value block.
- **What it does:** Reports a changing value from a sensor or the robot's memory while the program runs.
- **Where it can be used:** It fits into matching oval or rectangular input slots.
- **Example:** Use a location sensor reporter to get the robot's X-coordinate.

### Boolean / Hexagonal Block

- **Shape/Type:** Hexagonal Boolean block.
- **What it reports:** It reports one of two answers: `TRUE` or `FALSE`.
- **Why it has a different shape:** The shape helps show that it can only be used where a yes-or-no condition is needed.
- **Example:** `front eye detects blue?` can report `TRUE` when blue is detected and `FALSE` when it is not.

### Repeat Block

- **Shape/Type:** C-shaped loop block with a number input.
- **What it does:** Repeats the blocks inside it a specific number of times.
- **What goes inside:** Rectangular command blocks or other blocks that can run repeatedly.
- **Example:** Put `turn right` inside `repeat (4)` to turn right four times.

### Wait Until Block

- **Shape/Type:** Stack command block with a Boolean input.
- **What it does:** Pauses the program at that point until its condition becomes `TRUE`.
- **What kind of condition it needs:** It needs a hexagonal Boolean condition.
- **Example:** Wait until the distance sensor detects an object closer than 100 millimeters, then stop waiting and continue.

### If Then Block

- **Shape/Type:** C-shaped conditional control block, **not** a hexagonal block.
- **What it does:** Runs the blocks inside it only when its condition is `TRUE`.
- **What goes inside:** A hexagonal condition goes in the input slot, and command blocks go inside the C-shaped area.
- **Example:** If the front eye detects green, then drive forward.

> **Important:** The `if then` block is C-shaped. Only the condition placed inside it is hexagonal because that condition reports `TRUE` or `FALSE`.

### Forever Block

- **Shape/Type:** Long, C-shaped loop block.
- **What it does:** Repeats everything inside it continuously until the program is stopped.
- **Example:** Use `forever: if the front eye detects no color, drive forward` so the robot keeps checking and moving.

### Drive Forward Block

- **Shape/Type:** Rectangular stack/command block.
- **What it does:** Makes the VR Robot drive forward until another command stops it or changes its movement.
- **Example:** Put `drive forward` under the starter block to make the robot move across the arena.

## Concepts

### Sequence

The sequence of code matters because the robot follows commands from top to bottom in the exact order they are connected. A turn placed before a drive command produces a different result than a turn placed after it.

### Parameters

A parameter is an editable input, such as a number, distance, speed, or direction, that changes how a command behaves. For example, changing a drive distance from 200 mm to 500 mm makes the robot travel farther.

### Loops / Iteration

Loops, such as `repeat` and `forever`, run a group of blocks more than once. Iteration means one pass through the repeated instructions. Loops save time because the same commands do not need to be copied many times.

### Sensors

Sensors collect information about the robot's environment. For example, the Distance Sensor, Bumper Sensor, Eye Sensor, and Gyro provide information that the program can use to make decisions.

### Booleans & Conditions

A Boolean condition has only two possible answers: `TRUE` or `FALSE`. Hexagonal blocks often represent these conditions, such as whether a bumper is pressed or whether an eye detects a color.

### Sense → Think → Act

This is the basic robotic process. The robot **senses** information, **thinks** by checking a condition or making a comparison, and **acts** by running a command such as driving or turning.

### Comparisons

Comparison blocks use symbols such as `<`, `>`, and `=` to compare values. The result is a Boolean answer. For example, `distance < 100` is `TRUE` when an object is closer than 100 millimeters.

### Coordinates

VEXcode VR playgrounds use a two-dimensional coordinate system. The X-axis measures left and right, and the Y-axis measures forward and backward. A location can be described with an X-coordinate and a Y-coordinate.

### Conditionals

Conditionals, such as `if then` and `if then else`, let a program choose what to do based on a condition. This allows the robot to react differently in different situations.

### Patterns

A pattern is a behavior that repeats or follows a recognizable structure. Recognizing patterns helps you design algorithms, choose useful loops, and avoid writing the same commands repeatedly.

## Vocabulary

<details>
<summary><strong>VR Robot, Playground</strong></summary>

**Definition:**  
A **VR Robot** is a virtual robot that can be programmed to move, sense, and act. A **Playground** is the virtual arena where the VR Robot runs its program.

**In My Own Words:**  
The VR Robot is the character I control with code, and the Playground is the virtual world where it drives and completes challenges.

**Example:**  
I can program the VR Robot to drive through a maze in the Playground.

</details>

<details>
<summary><strong>Programming Language, Project</strong></summary>

**Definition:**  
A **Programming Language** is a system for writing instructions that a computer or robot can understand. A **Project** is the saved collection of code and settings used to solve a task.

**In My Own Words:**  
The programming language is how I communicate with the robot, and the project is the complete piece of work I create and save.

**Example:**  
I can use VEXcode Blocks as the programming language in a project that makes the VR Robot collect objects.

</details>

<details>
<summary><strong>Behavior, Command</strong></summary>

**Definition:**  
A **Behavior** is something the robot does, such as moving or turning. A **Command** is one instruction that tells the robot to perform an action.

**In My Own Words:**  
A command is a single direction, and a behavior is the action or result I see when the robot follows one or more commands.

**Example:**  
The command `drive forward for 200 mm` creates the behavior of the robot moving forward.

</details>

<details>
<summary><strong>Drivetrain</strong></summary>

**Definition:**  
The **Drivetrain** is the part of the VR Robot that controls movement, including driving forward, driving backward, and turning.

**In My Own Words:**  
The drivetrain is the robot's movement system. I use drivetrain blocks whenever I want the robot to travel or change direction.

**Example:**  
A drivetrain command can make the robot drive forward 300 millimeters and then turn right.

</details>

<details>
<summary><strong>Loop, Iteration</strong></summary>

**Definition:**  
A **Loop** repeats a group of instructions. An **Iteration** is one time through the instructions inside the loop.

**In My Own Words:**  
A loop is the repeat instruction, while an iteration is each individual repeat that actually happens.

**Example:**  
A `repeat (3)` loop has three iterations of the blocks inside it.

</details>

<details>
<summary><strong>Sensor, Bumper Sensor</strong></summary>

**Definition:**  
A **Sensor** detects information about the robot or its environment. A **Bumper Sensor** detects whether the robot's bumper is being pressed.

**In My Own Words:**  
Sensors help the robot learn what is happening. The Bumper Sensor is like a touch switch that answers whether the robot has bumped into something.

**Example:**  
If the Bumper Sensor is pressed, the program can stop the robot and turn it away from the wall.

</details>

<details>
<summary><strong>Boolean, Condition, TRUE/FALSE</strong></summary>

**Definition:**  
A **Boolean** is a value that can only be `TRUE` or `FALSE`. A **Condition** is a question or statement that produces a Boolean result. `TRUE` means the condition is correct or happening, while `FALSE` means it is not.

**In My Own Words:**  
The program checks a condition like a yes-or-no question. The answer is either `TRUE` or `FALSE`, and the program can use that answer to decide what to do.

**Example:**  
A Bumper Sensor can be used to check whether the bumper is pressed.

`Pressed = TRUE`  
`Not pressed = FALSE`

</details>

<details>
<summary><strong>Distance Sensor, Threshold</strong></summary>

**Definition:**  
A **Distance Sensor** measures how far an object is from the robot. A **Threshold** is a chosen limit used to decide when something should happen.

**In My Own Words:**  
The distance sensor tells the robot how far away something is, and the threshold is the cutoff number used for a decision.

**Example:**  
If the distance sensor reads less than the threshold of 100 millimeters, the robot can stop.

</details>

<details>
<summary><strong>Coordinate Plane, X-axis, Y-axis, X-coordinate, Y-coordinate</strong></summary>

**Definition:**  
A **Coordinate Plane** is a grid used to describe locations. The **X-axis** runs left and right, and the **Y-axis** runs forward and backward. An **X-coordinate** gives a location's position on the X-axis, while a **Y-coordinate** gives its position on the Y-axis.

**In My Own Words:**  
The coordinate plane is the map. The X-coordinate tells how far left or right a point is, and the Y-coordinate tells how far forward or backward it is.

**Example:**  
The location `(200, -100)` has an X-coordinate of `200` and a Y-coordinate of `-100`.

</details>

<details>
<summary><strong>Location Sensor</strong></summary>

**Definition:**  
A **Location Sensor** reports where the VR Robot is on the Playground, including its X-coordinate, Y-coordinate, and often its direction.

**In My Own Words:**  
The location sensor works like a map for the robot. It lets the program check where the robot is and decide where it should go next.

**Example:**  
The robot can drive until its X-coordinate is greater than 500, then stop.

</details>

<details>
<summary><strong>Comment</strong></summary>

**Definition:**  
A **Comment** is a note in a program that explains the code but does not make the robot perform an action.

**In My Own Words:**  
A comment is a reminder for people reading the project. It can explain what a group of blocks is supposed to do.

**Example:**  
`// Drive to the first wall` explains the next part of a program without changing how the robot runs.

</details>

<details>
<summary><strong>Eye Sensor</strong></summary>

**Definition:**  
The **Eye Sensor** detects visual information, such as colors, objects, and whether the robot can see an object in front of it.

**In My Own Words:**  
The Eye Sensor is the robot's camera-like sensor. It helps the robot react to colors and objects that it sees.

**Example:**  
If the Eye Sensor detects green, the robot can turn left.

</details>

<details>
<summary><strong>Conditional Statement</strong></summary>

**Definition:**  
A **Conditional Statement** tells a program to run different instructions depending on whether a condition is `TRUE` or `FALSE`.

**In My Own Words:**  
A conditional is a decision in the code: if something is true, do one action; otherwise, do nothing or do a different action.

**Example:**  
`if distance < 100, then stop` is a conditional statement because the robot stops only when the condition is true.

</details>

## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.

This ensures your notes are easy for you and others to read later.

---

## Headings

**When to use:** Organize your notebook into sections, such as days, topics, or projects.

- `#` for the notebook title; use it once at the top.
- `##` for each day or major topic.
- `###` for subsections such as Notes, Practice, or Reflections.

# Example:

# My Coding Notebook

## Day 1

### Notes

### Practice

## Text Formatting

Use bold for key terms or definitions, italics for emphasis or side comments, and inline code for keywords, functions, or commands.

# Example:

**Class** = a blueprint for objects  

*Remember:* always test your code  

Use `System.out.println()` to print.

## Code Blocks

Use fenced code blocks with a language name whenever you write multiple lines of code. Use inline code for short snippets.

# Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

## Lists

Use numbered lists for sequences or steps and bulleted lists for unordered ideas.

1. Define the class.
2. Write the main method.
3. Test your program.

- Variables
- Loops
- Conditionals

## Checklists

Use checklists to track progress on assignments or tasks.

- [x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

## Blockquotes

Use blockquotes for notes, reminders, or teacher comments.

> 💡 Remember: Loops repeat code until a condition is false.

## Tables

Use tables to compare values, track progress, or organize data neatly.

| Task | Status | Notes |
|---|---|---|
| Homework 1 | Done | Submitted |
| Homework 2 | Pending | Needs review |

## Links & Images

Use links and images when they help explain an idea.

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)

![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

To make an image a link, put `<a href="website address">` before the image and `</a>` after it.

## Collapsible Sections

Use collapsible sections to hide solutions or extended notes.

# Example:

<details>
<summary>Click to reveal solution</summary>

`System.out.println("Answer: 42");`

</details>

## Footnotes

Use footnotes for references or side notes without cluttering the page.

This concept is related to object-oriented programming.[^1]

[^1]: See “Objects and Classes” in your textbook.

## Style Rules

- Consistency matters more than creativity.
- Always use headings to structure your notes.
- Always use code blocks for multi-line code.
- Bold key terms.
- Use lists instead of long sentences when outlining steps.
- Use a professional tone.
- Use blockquotes for reflections or teacher feedback.
- Use checklists to mark progress.
- Use collapsible sections if you want to hide answers until review time.

## Bottom Line

- Headings = Structure
- Bold/Italic = Emphasis
- Code blocks = Code
- Lists = Steps/Ideas
- Tables = Organization
- Checklists = Progress
- Blockquotes = Notes/Tips
- Collapsible sections = Hide/Show detail

Keep it simple, consistent, and clear.
