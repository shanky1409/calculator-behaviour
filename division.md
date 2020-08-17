# Division Scenario

## Scenario: Division of two positive number
  
  Given that I turn on the calculator
  
  When I type in "positive number"
  And I press "division operator"
  And I type in "positive number"
  And I press "equals"
  
  Then I see the "subtracted number" as the result

## Scenario: Division of two negative number
  
  Given that I turn on the calculator
  
  When I type in "negative number"
  And I press "division operator"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the "subtracted number" as the result

## Scenario: Division of two fraction number
  
  Given that I turn on the calculator
  
  When I type in "fraction number"
  And I press "division operator"
  And I type in "fraction number"
  And I press "equals"
  
  Then I see the "subtracted number in fraction" as the result

## Scenario: Division of two decimal number
  
  Given that I turn on the calculator
  
  When I type in "decimal number"
  And I press "division operator"
  And I type in "decimal number"
  And I press "equals"
  
  Then I see, "subtracted number with precision up to 2 digits" as the result

## Scenario: Division of positive and negative number
  
  Given that I turn on the calculator
  
  When I type in "positive number"
  And I press "division operator"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the "subtracted number" as the result

## Scenario: Typing operators more than once
  
  Given that I turn on the calculator
  
  When I type in "positive/negative number"
  And I press "division operator twice"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then consider the last operator

## Scenario: Division is not symmetric
  
  Given that I turn on the calculator
  
  When I type a unique "positive/negative number(A)"
  And I press "division operator"
  And I type in another unique "positive/negative number(B)"
  And I press "equals"
  
  Then the number is not equal to "(B / A)"

## Scenario: Division with first number as 0
  
  Given that I turn on the calculator
  
  When I type in "0"
  And I press "division operator"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then I see 0 as the result

## Scenario: Division with second number as 0
  
  Given that I turn on the calculator
  
  When I type in "positive/negative number"
  And I press "division operator"
  And I type in "0"
  And I press "equals"
  
  Then I see error message as "Division by 0 is not allowed"

## Scenario: Division with both number as 0
  
  Given that I turn on the calculator
  
  When I type in "0"
  And I press "division operator"
  And I type in "0"
  And I press "equals"
  
  Then I see error message as "Division by 0 is not allowed"

## Scenario: Division of Identity operation
  
  Given that I turn on the calculator
  
  When I type in "positive/negative number"
  And I press "division operator"
  And I type in "1"
  And I press "equals"
  
  Then I see that the positive/negative number as the result
