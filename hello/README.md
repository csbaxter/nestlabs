# Hello

{% video https://www.youtube.com/watch?v=DmE9lCvrxgU %}

{% next %}

## Our First C Program!

Shall we have you write your first program? In the file named hello.c, write your first program by typing precisely these lines into the file on the line in between the curly brackets:

```c
printf("hello, world\n");
```

so that your file looks like:

```c
#include <stdio.h>

int main(void)
{
    printf("hello, world\n");
}
```

{% next %}

## Compiling Programs

Now, before we can execute the program at right, recall that we must *compile* it with a *compiler*, translating it from *source code* into *machine code* (i.e., zeroes and ones). Execute the command below to do just that:

```
make hello
```

And then execute this one again:

```
ls
```

This time, you should see not only `hello.c` but `hello` listed as well? (You can see the same graphically if you click that folder icon again.) That's because `make` has translated the source code in `hello.c` into machine code in `hello`, which happens to be the zeros and ones that the computer understands.

Now run the program by executing the below.

```
./hello
```

Hello, world, indeed!

## Testing with `check50`

<style type="text/css">
#red {color:red;}
#green {color:green;}
#orange {color:orange;}
#good {color: green;}    
</style>

To evaluate the correctness of your code, type in the following after the dollar prompt `$` in the terminal below your code. Log in with your GitHub username and password when prompted. For security, you'll see asterisks (`*`) instead of the actual characters in your password.

```
check50 cs50/problems/2019/ap/hello
```
Assuming your program is correct, you should then see output like:

<div id="green">
<pre><code>:) syntax.c exists.<br/>
:) syntax.c compiles.<br/>
:) prints "This is CS50AP!\n"</code></pre>
</div>

If you instead see yellow or red smileys, it means your code isn’t correct! For instance, suppose you see something like this:

<div><pre>
<span id="green">:) syntax.c exists.</span>
<span id="red">:( syntax.c compiles.
    expected exit code 0, not 1</span>
<span id="orange">:| prints "This is CS50AP!\n"
    can't check until a frown turns upside down</span>
</pre></div>

Because check50 is not able to compile style.c, as per the red smiley, odds are you still have an error in your syntax. The other yellow smiley, means that the check is dependent on sytax.c compiling, and so it wasn’t even run.

{% next %}

### Styling with `style50`

Though C doesn't care about how you style your code (in other words code with correct syntax but inconsistent spacing will compile and execute), CS50 does! That's because spacing your code consistently makes it easier to read and as we'll see soon, easier to debug.

You can check that your spacing is correct by executing the following at the `$` prompt:

```
style50 syntax.c
```

If there’s room for improvement in your code’s style, highlighted in red will be any characters you should delete, and highlighted in green will be any characters you should add.

When style50 ouputs:

<div id="green">
    <pre><code>Looks good!</code></pre>
</div>

you are done!

{% next "Ready to Submit?" %}

## How to Submit

Type the line below into your terminal to submit. For security, you'll see asterisks (`*`) instead of the actual characters in your password.

```
submit50 cs50/2018/ap/hello
```

