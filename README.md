# Scenarios

## Scenario1 - Allow Program being closed when x being pressed

| Input Sequence | Expected Output  |
| -------------- | ---------------- |
| x              | Exit the program |
| X              | Exit the program |

## Scenario2 - Add Customer

### 2.1 Invalid input provided

| Input Sequence             | Expected Output                                                              |
| -------------------------- | ---------------------------------------------------------------------------- |
| 4                          | prompt on adding customer name                                               |
| invalid name given         | error messaged prompted and error is handled                                 |
| valid name given           | phone number input message prompted                                          |
| invalid phone number given | error messaged prompted and error is handled                                 |
| valid phone number given   | email input message prompted                                                 |
| invalid email given        | error messaged prompted and error is handled                                 |
| valid email given          | prompt message to indicate customer has been added and navigate to main menu |
| 1                          | newly added customer should be displayed                                     |

### 2.2 All empty input provided

| Input Sequence             | Expected Output                                                              |
| -------------------------- | ---------------------------------------------------------------------------- |
| 4                          | prompt on adding customer name                                               |
| invalid name given         | error messaged prompted and error is handled                                 |
| empty name given           | phone number input message prompted                                          |
| invalid phone number given | error messaged prompted and error is handled                                 |
| empty phone number given   | email input message prompted                                                 |
| invalid email given        | error messaged prompted and error is handled                                 |
| empty email given          | prompt message to indicate customer has been added and navigate to main menu |
| 1                          | newly added customer should be displayed with all fields showing empty       |

### 2.3 empty name input provided

| Input Sequence             | Expected Output                                                              |
| -------------------------- | ---------------------------------------------------------------------------- |
| 4                          | prompt on adding customer name                                               |
| invalid name given         | error messaged prompted and error is handled                                 |
| empty name given           | phone number input message prompted                                          |
| invalid phone number given | error messaged prompted and error is handled                                 |
| valid phone number given   | email input message prompted                                                 |
| invalid email given        | error messaged prompted and error is handled                                 |
| valid email given          | prompt message to indicate customer has been added and navigate to main menu |
| 1                          | newly added customer should be displayed with name field showing empty       |

### 2.4 empty phone number input provided

| Input Sequence             | Expected Output                                                                |
| -------------------------- | ------------------------------------------------------------------------------ |
| 4                          | prompt on adding customer name                                                 |
| invalid name given         | error messaged prompted and error is handled                                   |
| valid name given           | phone number input message prompted                                            |
| invalid phone number given | error messaged prompted and error is handled                                   |
| empty phone number given   | email input message prompted                                                   |
| invalid email given        | error messaged prompted and error is handled                                   |
| valid email given          | prompt message to indicate customer has been added and navigate to main menu   |
| 1                          | newly added customer should be displayed with phone number field showing empty |

### 2.5 empty phone number input provided

| Input Sequence             | Expected Output                                                              |
| -------------------------- | ---------------------------------------------------------------------------- |
| 4                          | prompt on adding customer name                                               |
| invalid name given         | error messaged prompted and error is handled                                 |
| valid name given           | phone number input message prompted                                          |
| invalid phone number given | error messaged prompted and error is handled                                 |
| valid phone number given   | email input message prompted                                                 |
| invalid email given        | error messaged prompted and error is handled                                 |
| empty email given          | prompt message to indicate customer has been added and navigate to main menu |
| 1                          | newly added customer should be displayed with email field showing empty      |

## Scenario 3 - List All Services and Parts

| Input Sequence                             | Expected Output                               |
| ------------------------------------------ | --------------------------------------------- |
| 2                                          | all services listed in **alphabetical** Order |
| Modify the data file by swapping part name | -                                             |
| 3                                          | all parts listed in **alphabetic** order      |

## Scenario 4 - Add a job

### 4.1 No user selected

| Input Sequence                         | Expected Output                                                                                                 |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| 5                                      | a list of available customer displayed(for better user experience) and ask user to choose from an existing user |
| none existing user/empty user provided | ask the user to choose again or exit to the main menu                                                           |
| exit                                   | back to the main menu                                                                                           |

### 4.2 empty service and empty parts provided

| Input Sequence                         | Expected Output                                                                                                 |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| 5                                      | a list of available customer displayed(for better user experience) and ask user to choose from an existing user |
| none existing user/empty user provided | ask the user to choose again or exit to the main menu                                                           |
| valid user provided                    | a list of services displayed and ask the user to choose one                                                     |
| invalid service selected               | ask the user to re-select or continue                                                                           |
| continue                               | a list of parts displayed and ask the user to choose one                                                        |
| invalid part selected                  | ask the user to re-select or continue                                                                           |
| continue                               | amount should be 0, paid flag should be false and the job with today's date as key has been added               |
| exit                                   | back to the main menu                                                                                           |

### 4.3 empty service and multiple parts provided

| Input Sequence                         | Expected Output                                                                                                      |
| -------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| 5                                      | a list of available customer displayed(for better user experience) and ask user to choose from an existing user      |
| none existing user/empty user provided | ask the user to choose again or exit to the main menu                                                                |
| valid user provided                    | a list of services displayed and ask the user to choose one                                                          |
| invalid service selected               | ask the user to re-select or continue                                                                                |
| continue                               | a list of parts displayed and ask the user to choose one                                                             |
| invalid part selected                  | ask the user to re-select or continue                                                                                |
| valid part selected                    | ask the user to select or continue                                                                                   |
| valid part selected                    | ask the user to select or continue                                                                                   |
| continue                               | amount should be correctly calculated, paid flag should be false and the job with today's date as key has been added |
| exit                                   | back to the main menu                                                                                                |

### 4.4 multiple service and empty parts provided

| Input Sequence                         | Expected Output                                                                                                      |
| -------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| 5                                      | a list of available customer displayed(for better user experience) and ask user to choose from an existing user      |
| none existing user/empty user provided | ask the user to choose again or exit to the main menu                                                                |
| valid user provided                    | a list of services displayed and ask the user to choose one                                                          |
| invalid service selected               | ask the user to re-select or continue                                                                                |
| valid service selected                 | ask the user to select or continue                                                                                   |
| valid service selected                 | ask the user to select or continue                                                                                   |
| continue                               | a list of parts displayed and ask the user to choose one                                                             |
| invalid part selected                  | ask the user to re-select or continue                                                                                |
| continue                               | amount should be correctly calculated, paid flag should be false and the job with today's date as key has been added |
| exit                                   | back to the main menu                                                                                                |

### 4.5 multiple service and multiple parts provided

| Input Sequence                         | Expected Output                                                                                                      |
| -------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| 5                                      | a list of available customer displayed(for better user experience) and ask user to choose from an existing user      |
| none existing user/empty user provided | ask the user to choose again or exit to the main menu                                                                |
| valid user provided                    | a list of services displayed and ask the user to choose one                                                          |
| invalid service selected               | ask the user to re-select or continue                                                                                |
| valid service selected                 | ask the user to select or continue                                                                                   |
| valid service selected                 | ask the user to select or continue                                                                                   |
| continue                               | a list of parts displayed and ask the user to choose one                                                             |
| invalid part selected                  | ask the user to re-select or continue                                                                                |
| valid part selected                    | ask the user to select or continue                                                                                   |
| valid part selected                    | ask the user to select or continue                                                                                   |
| continue                               | amount should be correctly calculated, paid flag should be false and the job with today's date as key has been added |
| exit                                   | back to the main menu                                                                                                |

## Scenario 5 - List Unpaid Bills

| Input Sequence | Expected Output                                                                 |
| -------------- | ------------------------------------------------------------------------------- |
| 6              | all unpaid bills with customer name, phone number, date, amount being displayed |
| exit           | back to the main menu                                                           |

## Scenario 6 - Pay bills

### 6.1 Pay bill successfully

| Input Sequence            | Expected Output                                                                  |
| ------------------------- | -------------------------------------------------------------------------------- |
| 7                         | dispaly a list of customers and ask to select one                                |
| invalid customer provided | ask to reselect or exit                                                          |
| valid customer selected   | display a list of unpaid jobs for the customer and ask user to choose one to pay |
| choose an invalid job     | ask user to re-select or cancel payment                                          |
| choose a valid job        | show end user that the payment was sucessful                                     |
| exit                      | back to the main menu                                                            |

### 6.2 not choosing a customer

| Input Sequence            | Expected Output                                   |
| ------------------------- | ------------------------------------------------- |
| 7                         | dispaly a list of customers and ask to select one |
| invalid customer provided | ask to reselect or exit                           |
| exit                      | back to the main menu                             |

### 6.3 Pay bill unSuccessfully

| Input Sequence            | Expected Output                                                                  |
| ------------------------- | -------------------------------------------------------------------------------- |
| 7                         | dispaly a list of customers and ask to select one                                |
| invalid customer provided | ask to reselect or exit                                                          |
| valid customer selected   | display a list of unpaid jobs for the customer and ask user to choose one to pay |
| choose an invalid job     | ask user to re-select or cancel payment                                          |
| cancel payment            | show end user that the payment was cancelled                                     |
| exit                      | back to the main menu                                                            |
