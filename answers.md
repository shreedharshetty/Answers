First Steps Questionnaire with Answers
======================================

As the first step in our getting to know each other, please take a moment to
send your answers to the questions below to
[work@dispatch.tv](mailto:work@dispatch.tv). Feel free to include just your
answers or, if you prefer, just download this file (click the "Raw" button at
the top of this github page) and include your answers directly inline.

For JavaScript questions, assume that you are using version 1.8.5 of the
language as described [at
Mozilla](https://developer.mozilla.org/en-US/docs/JavaScript/Reference).

1. What is the result of the following block of JavaScript code:
    
        ( function f( x, y, m ) {
    
            if ( m > 0 ) { return f( y, x + y, m - 1 ); }
            return y;
    
        }( 1, 2, 7 ) );
	Answer is : 55
		f(1,2,7)
		 ==> f(2, 3, 6) 
		 	==> f(3, 5, 5) 
		 		==> f(5, 8, 4) 
		 			==> f(8, 13, 3) 
		 				==> f(13, 21, 2) 
		 					==> f( 21, 34, 1) 
		 						==> f(34, 55, 0) 
		 							==> 55
2. Given the following HTML fragments, what are the visual differences between
the two:
    	
        <!-- Option A -->
        <div>
            <p id="p1">Hello</p>
            <p id="p2" style="visibility:hidden">my</p>
            <p id="p3">friend</p>
        </div>
    
        <!-- Option B -->
        <div>
            <p id="p1">Hello</p>
            <p id="p2" style="display:none">my</p>
            <p id="p3">friend</p>
        </div>
    Answer is : 
    	In the option A, there will be empty line between p with id p1 and p with id p3, reason for this is whenever the element is having style 'visibility : hidden', the element hold the space and present in the DOM and hidden.

    	output looks something like this :
    		Hello

    		Friend
    	In the option B, there wont be any empty line between p with id p1 and p3, reason for this is whenever the element is having style 'display:none', it wont hold the space but it will be hidden in the DOM.

    	output looks something like this :
    		Hello
    		Friend

3. Given the following block of JavaScript:
    
        var o = { a: 1, b: "1.0", c: false, d: true };
        var a = "b";
    
   what are the results of the following expressions:
    
        o.a ==> 1
        o[ a ] ==> 1.0
        o.a == o.b ==> true // == will not make the type check
        o.a === o.b ==> false // integer 1 is not same as string 1.0
        o.b == o.d ==> true // string comparison with boolean true always return true // if we use === returns false
        o.a === o.d ==> false // here type check also happens
        o.c ? "a" : "b" ==> "b" // o.c is false so else block will execute
        o.e ==> undefined  // as key 'e' is not present in the o
        o.e === null ==> false
        o.e != null ==> false

4. What is the result of the following unix shell command (feel free to run it
from a terminal to find out):

        printf "ab\ncd\ncc\n" | grep -v d | tr 'a' 'Z'

   Explain, briefly, how each piece of the command contributes to the result.

   answer : 
   		printf "ab\ncd\ncc\n" prints
   		ab
   		cd
   		cc

   		grep -v d finds the matched line which has d in it, since we are using -v here, it excludes the line which has d and returns
   		ab
   		cc

   		tr 'a' 'Z' will replace 'a' with 'Z'

   		so printf "ab\ncd\ncc\n" | grep -v d | tr 'a' 'Z' 
   		returns 
   		Zb
   		cc


5. Create, Register, and Confirm an account using our [iOS
app](https://itunes.apple.com/us/app/dispatch.tv/id690762433?mt=8) or [the
website](http://www.dispatch.tv) (Note: registration page for the web can be
found [here](http://www.dispatch.tv/register)). Once you're in, create a channel
with your name as the title and add the user `work@dispatch.tv` to your channel.
Because every channel requires at least one video or one text comment, use this
as an opportunity to tell us something you like about the app, and something
that you think should change or which could be done better. Please limit your
response to 500 characters or, if responding with a video, 30 seconds.

Answer : 
	Sign in button seems so dull when it is disabled, UI needs some more charm, as i see header seems so dull.
	In the conversation page, form controls need to be buttons.
	Page looks so plain.
	wouldn't it be better if we place the logo in top as usual? or is there a specific reason to place logo in the bottom?
	Width of the page also looks less.
	About us page is asking me to login again though i am logged in.
	Design of the about-us page is looking little nice than landing page.



6. After you've used the app a little bit, step back and think about it in the
world at large. How would you use it? How would you explain it to other people
in 2 sentences? If you had to sell it as a productivity tool, who would you sell
it to (Nurses and doctors? Construction companies? Retail store managers?)
Please limit your answer to 500 characters.

Answer : 
	I would like to use it to broadcast my friends and family about my status, place and share the video with them.
	I would like to explain it to my friends/family like dispatch.tv is personalized socialize platform to share what i have discovered.
	It can also be used in a team of developers, where they can share all the excitements of writing cool stuff.
	
	