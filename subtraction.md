# Subtraction

## Scenario: Subtraction of two positive number
  
  Given that I turn on the calculator
  
  When I type in "positive number"
  And I press "minus"
  And I type in "positive number"
  And I press "equals"
  
  Then I see the "subtracted number" as the result

## Scenario: Subtraction of two negative number
  
  Given that I turn on the calculator
  
  When I type in "negative number"
  And I press "minus"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the "subtracted number" as the result

## Scenario: Subtraction of two fraction number
  
  Given that I turn on the calculator
  
  When I type in "fraction number"
  And I press "minus"
  And I type in "fraction number"
  And I press "equals"
  
  Then I see the "subtracted number in fraction" as the result

## Scenario: Subtraction of two decimal number
  
  Given that I turn on the calculator
  
  When I type in "decimal number"
  And I press "minus"
  And I type in "decimal number"
  And I press "equals"
  
  Then I see, "subtracted number with precision up to 2 digits" as the result

## Scenario: Subtraction of positive and negative number
  
  Given that I turn on the calculator
  
  When I type in "positive number"
  And I press "minus"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the "subtracted number" as the result

## Scenario: Typing operators more than once
  
  Given that I turn on the calculator
  
  When I type in "positive/negative number"
  And I press "minus twice"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then consider only the last operator

## Scenario: Subtraction is not symmetric
  
  Given that I turn on the calculator
  
  When I type a unique "positive/negative number(A)"
  And I press "minus"
  And I type in another unique "positive/negative number(B)"
  And I press "equals"
  
  Then the number is not equal to "(B - A)"

## Scenario: Subtraction of Identity operation
  
  Given that I turn on the calculator
  
  When I type in "0"
  And I press "minus"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then I see that "negative/positive number" as the result
