# ft_containers testing guide

HI,
I'm here to guide you in using comprehensive testing for your project

here are some good testers you can test your code with

1) **ft_containers terminator :**
https://github.com/Mikastiv/ft_containers-terminator?ref=morioh.com&utm_source=morioh.com

It's a great tester, It has many decent tests for each costum container, it tracks the leaks and alive objects (objects that never got destroyed), and more than that, you can test each method separately and see the difference between your container and the container provided by the standard library

2) **ft_container UNITest :**
https://github.com/mamoussa405/ft_containers_tests

this tester does not just test the container with good tests, it also tests the time and speed of the methods provided by the container and compares it the built-in stl containers to see if your code is fast enough test with this tester but i personally like the first tester more since it provide more complex tests and leaks checking

## How To Use

i recommend starting with the second tester (UNITest) to get your hand dirty with testing and solve the basic riddles after you made sure that this tester
shows OK in all the test cases you can pass to the first tester which has some more complex and advanced test cases

1)

Run every tests: <br/>
`./test_containers.sh`

Run one or more container tests: <br/>
`./test_containers.sh <CONTAINER_1> ... <CONTAINER_N>`
<br/>Example: <br/>
`./test_containers.sh vector stack ...`

Run individual tests: <br/>
`./test_files.sh <CONTAINER> <TEST_1> ... <TEST_N>`
<br/>Example: <br/>
`./test_files.sh vector erase clear ...`

# Debug helper

You can create a executable (debug.out) for debugging a particular test with: <br/>
`./debug_test.sh <CONTAINER> <TEST>`
<br/>Example: <br/>
`./debug_test.sh vector erase`
