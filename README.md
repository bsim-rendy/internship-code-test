![BSIM Logo](https://www.banksinarmas.com/id/public/revamp/logoj.png;wa005ee3af0db84daa)


Developer Intern Coding Test
---
---

In this test, there are 2 problems that you need to solve.

The following programming languages could be used to solve the problems.
-   Java
-   Javascript

---

1.  Given _N > 0_. Transform _N_ into its reversed form.

    _Example Input:_
    *   _N_ = `12345`
        Then, reversed _N_ would be `54321`
    *   _N_ = `12300`
        Then, reversed _N_ would be `321`

    _Notes: reversed form needs to be a valid integer_
    
    From the following code section, you can add up to 3 lines of code and also change up to 3 lines of code to `solution` method in order to get the correct output to the problem described above.
    ```java
    public class Main {
        public static void main(String[] args) {
            solution(11011101);
            solution(-100);
            solution(521455130);
            solution(7451000);
        }
    
        static void solution(int N) {
            int enablePrint = 0;
            while (N > 0) {
                if (enablePrint == 0 && N % 10 != 1) {
                    enablePrint = N / 10;
                }
                if (enablePrint > 0) {
                    System.out.print(enablePrint);
                }
                N /= 10;
            }
            System.out.println();
        }
    }
    ```
    
    The expected output should be:
    ```bash
    10111011

    31554125
    1547
    ```
    
---
    
2.  A string _S_ consisting of _N_ characters is called properly nested if:
    -   _S_ is empty;
    -   _S_ has the form `"(U)"` where _U_ is a properly nested string;
    -   _S_ has the form `"VW"` where _V_ and _W_ are properly nested strings.
    
    For example, string `"(()(())())"` is properly nested but string `"())"` isn't.
    Write a function:
    
    ```javascript
    function solution(S);
    ```
    
    that, given a string _S_ consisting of _N_ characters, returns `1` if string _S_ is properly nested and `0` otherwise.
    
    For example, given `S = "(()(())())"`, the function should return `1` and given `S = "())"`, the function should return `0`, as explained above.
    
    Write an efficient algorithm for the following assumptions:
    -   _N_ is an integer within the range `[0..1,000,000]`;
    -   string _S_ consists only of the characters `"("` and/or `")"`.
    
---

_It would be nice to_:
-   include some comments on your code to explain your thought on the problem
-   send us your solution using git repository such as: GitHub, GitLab, BitBucket, etc
