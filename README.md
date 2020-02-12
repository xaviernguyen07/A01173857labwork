Q1: Is the keyword "fixes" the only way to auto-close an issue from a PR 
(pull request). Is there other keywords that can accomplish the same thing?
A1: You can link a pull request to an issue by using a supported keyword in the pull request's description.
close
closes
closed
fix
fixes
fixed
resolve
resolves
resolved

Q2: Do you have to create a new PR EVERYTIME you want to close an issue,
or is it possible to close multiple issues within a single PR? If so, 
how?
A2: According to what I found on stackoverflow. It is possible to close multiple issues within a single PR.
To close multiple issues, preface each issue reference with one of the above keywords. You must use the keyword before each issue you reference for the keyword to work.

For ex:This closes #34, closes #23, and closes example_user/example_repo#42 would close issues #34 and #23 in the same repository, and issue #42 in the "example_user/example_repo" repository.
For ex:
Summary of the change made.
Fixed following bugs:
* Modified error loader, fixes #1
* Returned a nonstale pointer, fixes #2
* Applied new graphics to gui elements, closes #3

Q3:Provide an example of using map that is different from the one I have done.
Your example must use map both as a named function declaration and with an
anonymous function. 
<p id="result"></p>

        <script>
		// anonymous function
		//The map() method creates a new array with the results of calling a function for every array element.
		//The map() method calls the provided function once for each element in an array, in order.

                let numbers = [2, 4, 9, 10, 12];
                let doubles = numbers.map(function (num) {
                        return num * 2;
                })

                document.getElementById("result").innerHTML = doubles;
        </script>

<p id="result"></p>
        <script>
		// a named function declaration
                <p id="result"></p>

        <script>
                let numbers = [2, 4, 9, 10, 12];
                function isEven(value) {
                        if (value % 2 == 0)
                                return true;
                        else
                                return false;
                }
                let new_array = numbers.map(isEven);
                document.getElementById("result").innerHTML = new_array;
        </script>

Why is the"transformation function" we discussed in class sometimes referred to as a callback function???

Because a callback function is a function that will be executed just after another function has finished executing.
Callback function is a function that is passed as an argument to another javascript function.