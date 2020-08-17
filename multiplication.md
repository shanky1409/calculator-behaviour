# Multiplication Scenario

## Scenario: Multiplication of two positive number
  
  Given that I turn on the calculator
  
  When I type in "positive number"
  And I press "multiply operator"
  And I type in "positive number"
  And I press "equals"
  
  Then I see the product of the numbers as the result

## Scenario: Multiplication of two negative number
  
  Given that I turn on the calculator
  
  When I type in "negative number"
  And I press "multiply operator"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the product of the numbers as the result

## Scenario: Multiplication of two fraction number
  
  Given that I turn on the calculator
  
  When I type in "fraction number"
  And I press "multiply operator"
  And I type in "fraction number"
  And I press "equals"
  
  Then I see the product of the numbers in fraction as the result

## Scenario: Multiplication of two decimal number
  
  Given that I turn on the calculator
  
  When I type in "decimal number"
  And I press "multiply operator"
  And I type in "decimal number"
  And I press "equals"
  
  Then I see, product of the numbers with precision up to 2 digit as the result

## Scenario: Multiplication of positive and negative number
  
  Given that I turn on the calculator
  
  When I type in "positive number"
  And I press "multiply operator"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the product of the numbers as the result

## Scenario: Typing operators more than once
  
  Given that I turn on the calculator
  
  When I type in "positive/negative number"
  And I press "multiply operator twice"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then consider the last operator

## Scenario: Multiplication is symmetric
  
  Given that I turn on the calculator
  
  When I type a unique "positive/negative number(A)"
  And I press "multiply operator"
  And I type in another unique "positive/negative number(B)"
  And I press "equals"
  
  Then the number is not equal to "(B * A)"

## Scenario: Multiplication with 0
  
  Given that I turn on the calculator
  
  When I type in "0"
  And I press "multiply operator"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then I see 0 as the result

## Scenario: Multiplication of Identity operation
  
  Given that I turn on the calculator
  
  When I type in "1"
  And I press "multiply operator"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then I see that the positive/negative number as the result
