# Java Exception Handling — Bank Withdrawal System

A beginner-friendly Java project demonstrating structured exception handling 
through a simulated bank withdrawal system.

## Concepts Covered
- try / catch / finally blocks
- Multi-catch syntax (IllegalArgumentException | ArithmeticException)
- Manually throwing exceptions using `throw`
- Declaring exceptions using `throws`

## How It Works
The `withdraw()` method validates the transaction and throws the appropriate 
exception if the amount is invalid or exceeds the balance. The caller handles 
it gracefully using multi-catch, and `finally` always confirms the attempt.

## Test Cases
| Scenario            | Input           | Result                          |
|---------------------|-----------------|---------------------------------|
| Valid withdrawal    | balance=1000, amount=400  | Withdrawn: 400.0, Remaining: 600.0 |
| Insufficient funds  | balance=1000, amount=2000 | Exception: Insufficient funds   |
| Invalid amount      | balance=1000, amount=-50  | Exception: Amount must be positive |

## Tech Stack
- Java (Core)
- Eclipse IDE
