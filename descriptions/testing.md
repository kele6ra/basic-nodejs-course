# Testing

Write tests for Ciphering machine CLI from 1st task.  
For writing tests [Jest](https://jestjs.io/) testing framework should be used.  

You can write simple unit tests on single functions (e.g. ciphering function, arguments parsing function, config validation function, etc.), mock some modules, test CLI using [child processes](https://nodejs.org/dist/latest-v14.x/docs/api/child_process.html) and so on.

## Scenarios

### Error scenarios
1) Input: User passes the same cli argument twice; Result: Error message is shown;
e.g. input: `node my_caesar_cli -c C1-C1-A-R0 -c C0` result: `Error: You provided -c argument more than once`;
2) Input: User doesn't pass -c or --config argument; Result: Error message is shown;
3) Input: User passes -i argument with path that doesn't exist or with no read access; Result: Error message is shown;
4) Input: User passes -o argument with path to directory that doesn't exist or with no read access; Result: Error message is shown;
5) Input: User passes incorrent symbols in argument for --config; Result: Error message is shown;

### Success scenarios
1) Input: User passes correct sequence of symbols as argument for --config that matches regular expression; Result: test passed
2) Take cipher usage scenarios from [first task description](https://github.com/AlreadyBored/basic-nodejs-course/blob/review-2021Q4/descriptions/caesar-cipher-cli-tool.md) usage examples.

## Minimal acceptance criteria
- Installed and used Jest framework (+0)
- Tests coverage is up to 70% (+20)
- All scenarios mentioned above are covered (+20)
- (+20)

## Additional acceptance criteria
- Used mock objects to test code (+20)
- Tests coverage is up to 90% (+20)

## Penalty points
- 


**MAX TOTAL SCORE: 100**
