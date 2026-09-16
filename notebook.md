## Table of Contents
- [Blocks](#blocks)
- [Concepts](#concepts)
- [Vocabulary](#vocabulary)
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)
  - [Headings](#headings)
  - [Text Formatting](#text-formatting)







## Blocks
Hat Block	
what it looks like: it looks like a hat
what it does: it starts off the code
where it belongs: at the top of the code

Stack / Command Block
what is does: it is a code where you can put other codes into it
how it connects to other commands: it connects by when you place it down in the code, you can put other codes inside of it and use the other code inside of that code

C-Block
what does the C- shape block mean: The C-shaped block means you are creating a loop or a conditional statement that controls when and how other blocks run.
why can other blocks be placed inside: Other blocks can be placed inside because C-blocks act as container rules for the instructions trapped inside them.

Reporter / Oval Block	
what is reports: A reporter block reports live, changing values from your robot's sensors or its memory while your program is running.
where it can be used: Reporter blocks in VEXcode VR can only be placed inside other blocks that have matching oval or rectangular slots.

Boolean / Hexagonal Block
What it reports: A Boolean block reports only one of two possible answers: True or False.
why it has a different shape: The hexagonal shape is a visual safety constraint designed to prevent coding mistakes

Repeat Block	
Its shape: The Repeat block is a C-shaped block (often colored orange) with a built-in input slot at the top. It features a top bump and a bottom notch to connect with standard code stacks, and its inner "mouth" automatically expands vertically as you add more blocks to it.
what it does: It repeats the actions nested inside it a specific number of times. Instead of manually copy-pasting the exact same blocks over and over, you type a number into the top input slot (like 4), and the block automatically loops through its contents that many times before letting the program move down to the next part of the code.
what goes inside it: Any standard, rectangular stack blocks (commands) go inside it.

Wait Until Block
What it does: The Wait Until block completely pauses the program's execution at that exact spot until a specific condition becomes true.
what kind of condition it needs: It needs a Boolean condition (a hexagonal block) that can be answered as either True or False.

If Then Block	Its shape, how its condition works, and what happens when the condition is TRUE

Forever Block
What is looks like: The forever block looks like a long stretched out C with bumps in the middle
What it does: it makes whatever code you put in it go on forever and never end
Example: i want the front eye for that whenever it detects no color it moves forward so i put (forever: if front eye detects nothing (drive forward))

For each block, include: a starter block at the top of the code

Name:
Shape/Type: drive forward block
What It Does: the drive forward block makes the car infinitely drive forward until stopped 
Example: i want to make the car drive forward all the way until the end of the arena so i used the dive forward block

Important
The If Then block is NOT hexagonal.

It is a C-shaped control block.

The condition that goes inside it is hexagonal because the condition reports either:

TRUE or FALSE





## Concepts








Sequence	Why the order of commands matters: The sequence of the code matters because robots can only do exactly what you tell them to do, in the precise order you list the commands from top to bottom.

Parameters	How changing an input changes what a command does: A parameter (or input) is the editable value inside a block—like a number, distance, speed, or direction—that tells the command exactly how to do its job. Without parameters, commands would be completely rigid. For example, a drive block wouldn't know whether to move one inch or one mile.

Loops / Iteration	How and why programs repeat instructions: Programs use loops (like repeat or forever C-blocks) to run a group of blocks multiple times without rewriting them. This matters because it saves time, keeps code clean, and allows the robot to perform continuous tasks (like constantly checking for obstacles while driving).

Sensors	How a robot gets information about its environment:  Sensors (like the Distance Sensor, Bumper Switches, and Gyro) send electronic signals to the robot’s brain about the virtual playground. This allows the robot to interact with the world dynamically instead of just driving blindly on a fixed timer.

Booleans & Conditions	How TRUE/FALSE information controls a program: A condition is a statement that is either True or False at any given moment (e.g., Bumper pressed = True). These hex-shaped blocks act as gates; if the condition is True, the program allows the robot to execute specific code, but if it is False, that code is blocked or skipped.

Sense → Think → Act	How a robot senses information, makes a decision, and responds:  This is the universal robotic loop. First, the robot Senses data from its environment (e.g., the front eye detects red). Next, its brain Thinks by evaluating that data against your code's logic rules. Finally, it Acts by sending power to its motors or tools based on that decision (e.g., it stops driving).

Comparisons	How < and > compare values and produce TRUE/FALSE:  Comparison blocks (green operators) take two changing numbers—like a live sensor value and a target number—and judge how they relate. For example, [Distance] < 50 constantly checks if the wall is closer than 50mm. The moment that statement becomes True, it triggers the next action in your code.

Coordinates	How X and Y values describe the robot's location: VEX VR playgrounds use a 2D grid system measured in millimeters, where the center is typically (0, 0). The X-axis tracks how far left (-) or right (+) the robot is, and the Y-axis tracks how far down (-) or up (+) it is, allowing you to program the robot to navigate to exact destinations on the map.

Conditionals	How programs make decisions using conditions: Conditionals (if-then and if-then-else blocks) create branching paths in your code. Instead of executing the exact same script every run, the robot evaluates a condition on the fly and chooses which path of instructions to follow based on what is happening around it.

Patterns	How recognizing repeated behavior can help create better algorithms:Conditionals (if-then and if-then-else blocks) create branching paths in your code. Instead of executing the exact same script every run, the robot evaluates a condition on the fly and chooses which path of instructions to follow based on what is happening around it.
























## Vocabulary





































  ## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  

This ensures your notes are easy for you (and others) to read later.

---

## Headings

**When to use:** Organize your notebook into sections (like days, topics, or projects).  

- `#` for the notebook title (use once at the top).  

- `##` for each day or major topic.  

- `###` for subsections (like "Notes", "Practice", "Reflections").  

# Example:

# My Coding Notebook

## Day 1

### Notes

### Practice

# Text Formatting

When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

# Example:

**Class** = a blueprint for objects  

*Remember:* always test your code  

Use `System.out.println()` to print

 

# Code Blocks

When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

# Example:

```java

public class Hello {

    public static void main(String[] args) {

        System.out.println("Hello World!");

    }

}

```

# Lists

When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

# Example:

Define the class
Write the main method
Test your program
Variables

- Loops

- Conditionals

 

# Checklists

When to use: Track progress on assignments or tasks.

# Example:

[x] Complete coding warm-up

- [ ] Finish project draft

- [ ] Reflect on learning

 

# Blockquotes

When to use: Call out notes, reminders, or teacher comments.

# Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

# Tables

When to use: Compare values, track progress, or organize data neatly.

# Example:

| Task        | Status   | Notes          |

|--------------|------------|-----------------| 

| Homework 1  | Done #  | Submitted      |

| Homework 2  | Pending  | Needs review   |

 

# Links & Images

When to use: Add references, resources, or visuals.

# Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  

![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

To make an image that is a link, paste the image, then add the following before it, replacing website address with the link:

<a href="website address">

And after the image info, add: </a>

# Collapsible Sections

When to use: Hide solutions, extended notes, or extra details.

# Example:

<details>

  <summary>Click to reveal solution</summary>

  

System.out.println("Answer: 42");

</details>

 

# Footnotes

When to use: Add references or side notes without cluttering the page.

# Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

# Style Rules

Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

# Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
