# Error logs dump in CI

## Installation
1. change the value of error_threshold value in to "1" in application/config/congig.php
2. change the value of db_debug to false in application/config/database.php
3. refer the lib_log file in system/libraries folder
4. add this file to libraries attribute of application/config/autoload.php
5. Apply the try and error logic in index function in application/controller/user.php file for testing
6. Apply the try catch logic for database errors in create_user function in application/model/user_model.php for testing
7. For testing URL : http://localhost/ci_error_log_db/user/register
8. Almost all the types of logs are dumped in log file as well as database.
9. We can dump database error logs using try catch
10. Some syntax error logs can dump in database if we used PHP 7 and used try catch in our code in any function.

