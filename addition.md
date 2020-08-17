# Addition

## Scenario: Addition of two positive number
  
  Given the calculator is turned on
  
  When I type in "positive number"
  And I press "plus"
  And I type in "positive number"
  And I press "equals"
  
  Then I see the "added number" as the result

## Scenario: Addition of two negative number
  
  Given the calculator is turned on
  
  When I type in "negative number"
  And I press "plus"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the "added number" as the result

## Scenario: Addition of two fraction number
  
  Given the calculator is turned on
  
  When I type in "fraction number"
  And I press "plus"
  And I type in "fraction number"
  And I press "equals"
  
  Then I see the "added number in fraction" as the result

## Scenario: Addition of two decimal number
  
  Given the calculator is turned on
  
  When I type in "decimal number"
  And I press "plus"
  And I type in "decimal number"
  And I press "equals"
  
  Then I see the "added number with precision up to 2 digits" as the result

## Scenario: Addition of positive and negative number
  
  Given the calculator is turned on
  
  When I type in "positive number"
  And I press "plus"
  And I type in "negative number"
  And I press "equals"
  
  Then I see the "added number" as the result

## Scenario: Typing operators more than once
  
  Given the calculator is turned on
  
  When I type in "positive/negative number"
  And I press "plus twice"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then I see the error message as invalid operation

## Scenario: Addition of Identity operation
  
  Given the calculator is turned on
  
  When I type in "0"
  And I press "plus"
  And I type in "positive/negative number"
  And I press "equals"
  
  Then I see that "positive/negative number" as the result
