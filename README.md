# Lab-5_202001180

                                                                    IT314
                                                          Software Engineering Lab-5
                                                               Static Analysis
                                            
**Name - Varshil Nayak**
**ID - 202001180**

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------


**Tool: Prospector**

**Code 1 : https://github.com/avinashkranjan/Amazing-Python-Scripts/blob/master/Age-Calculator-GUI/age_calc_gui.py**

- Errors:


![image](https://user-images.githubusercontent.com/124247649/225576171-005ea5f6-b84d-426f-acf3-58362b1d9adb.png)




**Analysis of errors:**
- Error for complex function
  - Functions that are deemed too complex are functions that have too much branching logic.
  - Line: 17
    mccabe: MC0001 / App.run is too complex (16)
- Error for no-else-return / Unnecessary "else" after "return"
  - This error comes when we use unncecassary else.
  - Line: 55 
    pylint: no-else-return / Unnecessary "else" after "return", remove the "else" and de-indent the code inside it (col 16)
- Error for Unused variables
  - This type of errors can be taken as warnings but we can solve this type of errors by trying to avoid declaring those type of variables.
  - Line: 61
    pylint: unused-variable / Unused variable 'e' (col 12)
 
**Code 2 : https://github.com/avinashkranjan/Amazing-Python-Scripts/blob/master/Coderforces_Problem_Scrapper/Codeforces_problem_scrapper.py**

- Errors:


![image](https://user-images.githubusercontent.com/124247649/225581596-0210ebe0-e770-40cb-ae66-d886df7e5380.png)




**Analysis of errors:**
- Error for import
  - For better practice in programming, we should use import at the toplevel means top of the code.
  -  Line: 2
    pylint: import-error / Unable to import 'selenium'
    
**Code 3 : https://github.com/avinashkranjan/Amazing-Python-Scripts/blob/master/Covid-19_Real-time_Notification/Covid.py**

- Errors:


![image](https://user-images.githubusercontent.com/124247649/225582753-f0a1e3f8-12d8-4217-8f16-81b21fed9475.png)
![image](https://user-images.githubusercontent.com/124247649/225582853-1f1cfae1-075d-4191-8b0a-f0fe0e112982.png)





**Analysis of errors:**
- Error for import
  - For better practice in programming, we should use import at the toplevel means top of the code.
  -  Line: 1
    pylint: import-error / Unable to import 'plyer'
    
- Error for bad indendation
  - This error occurs due to leaving more spaces.
  -  Line: 21
    pylint: bad-indentation / Bad indentation. Found 8 spaces, expected 4
    
**Code 4 : https://github.com/avinashkranjan/Amazing-Python-Scripts/blob/master/GST%20Calculator/script.py**

- Errors:


![image](https://user-images.githubusercontent.com/124247649/225583691-d56dbd44-8834-41fa-afa3-39fd89c7c015.png)
![image](https://user-images.githubusercontent.com/124247649/225583859-27029c0f-1983-402d-947f-5fc11e9018d4.png)






**Analysis of errors:**
- Error for import
  - For better practice in programming, we should use import at the toplevel means top of the code.
  -   Line: 1
    pylint: unused-wildcard-import / Unused imports from wildcard import: (s) 
    
- Error for undefined variable
  - This error occurs due to variable not defined at initialization.
  - Line: 6
    pyflakes: F405 / 'END' may be undefined, or defined from star imports: tkinter (col 32)
    

**Code 5 : https://github.com/avinashkranjan/Amazing-Python-Scripts/blob/master/Currency-Exchange-Rates/exchange_rates.py**

- Errors:


![image](https://user-images.githubusercontent.com/124247649/225584785-81eb2352-e934-422a-94b6-dcaa330cce71.png)







**Analysis of errors:**
- Error for f-string method
  - We could use % or the str.format method to format a string. Even though these methods are still valid, f-strings are more preferred.
  -   Line: 17
    pylint: consider-using-f-string / Formatting a regular string which could be a f-string (col 10)
