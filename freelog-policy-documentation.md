grammar:
 tree structure overview
# Concept
  + States:
  represent the a situation of a contract, a state can be a terminate state, an activate state or a intermediate state.
  + Events: represent an action that changes a state. There are multiple pre-defined events available.

# Events
+ ####transaction_event

  grammar: 'receiving transaction of' INT to FEATHERACCOUNT

  example: receiving transaction of 100 to 0x12345

+ ####signing_event
  grammar: 'signing license' ID

  example: signing license LicenseResourceId
+ ####period_event
  grammar: 'every' time_cycle

+ ####specific_date_event

   grammar: 'arriving date' DATE

+ ####relative_date_event

  grammar

+ ####guaranty_event
  grammar: 'having deposit of' INT
+ ####access_count_event
  grammar: 'reaching 100 use'

+ ####per access_count_event
  grammar: 'per 100 use'
+ ####settlement_event

  pending
+ ####pricing_agreement_event
  pending

# Types
 + ## Enumerate
    + time_cycle

    + user group

       user_groups names are limited. There are only four types of user groups. AllVisiter, RegisteredUser, LoginUser, RegisteredNode.
  + ## Regular Expression
    + FEATHERACCOUNT

       FEATHERACCOUNT is account, it is either a 13-digit phone number or e-mail address.

       Regular Expression :[0-9a-zA-Z@.]+;
    + INT

       INT is non-negative integer.

    + ID

        ID are symbols that includes Upper Case, lower case or underscore.

        Regular Expression :([a-zA-Z]|'_')+;


  # Reserved words
  For

  initial

  proceed to

  on accepting

  AllVisiter

  RegisteredUser

  LoginUser

  RegisteredNode
