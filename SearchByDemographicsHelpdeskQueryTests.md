#Tests for search by demographics

##Existing tests

The existing tests rely on the Database.
The only two cases tested are:
        - ExactMatch_NotFuzzy
        - MultipleMatch_NotFuzzy
Both are testing duplicate entryes in the database. Only the ULN is changing.

##Missig test cases

- ExactMatch_Fuzzy (Multiple cases for different fields)
        * The test will pass to the query misspelled parameters, or synonym parameters  

- MultipleMatch_Fuzzy (Multiple cases for different fields)
        * The test will pass to the query misspelled parameters, or synonym parameters  

- ToManyResults
        * The test wll return the to many results response code. 


#Tests for search by demographics Helpdesk

FN   = Familly Name
GN   = Given Name
DOB  = Date Of Birth
PO   = Postcode
G    = Gender

- ExactMatch_NotFuzzy_FN_GN#
                           # _DOB
                           # _PO
                           # _DOB_PO
                           # _DOB_G
                           # _PO_G
                           # _DOB_PO_G

- MultipleMatch_NotFuzzy

- ExactMatch_Fuzzy
        *This will have Test Cases where synonyms values or misspelled values for the fields will be passed

- MultipleMatch_Fuzzy