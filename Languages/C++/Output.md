The `cout` object, together with the `<<` operator, is used to output values and print text.
# Newline
The newline character (`\n`) is called an **escape sequence**, and it forces the cursor to change its position to the beginning of the next line on the screen. This results in a new line. To insert a new line in your output, you can use the `\n` character:
![[Pasted image 20241023224827.png]]

You can also use another `<<` operator and place the `\n` character after the text, like this:
![[Pasted image 20241023224930.png]]
**Tip:** Two `\n` characters after each other will create a blank line:
![[Pasted image 20241023225950.png]]

Another way to insert a new line, is with the `endl` manipulator:
![[Pasted image 20241023225034.png]]
Examples of other valid escape sequences are:
![[Pasted image 20241023225915.png]]