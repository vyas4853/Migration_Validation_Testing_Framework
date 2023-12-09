# SAP TO DATABRICKS MIGRATION VALIDATION FRAMEWORK
This Framework is designed while migrating views and wrappers to databricks from SAP HANA.  I have used Pyspark and databricks SQL in this Framework.

Test this Framework consists.

Row count 
Column count
Duplicate record count
Null value count of grain columns
Sum of measured columns
Execution time of SAP view/Wrapper
Execution time of View/Wrapper in databricks

You have to pass parameters from another notebook to this farmework notebook.

Parameters should be passed from another notebook

%run ./Migration_Validation_Testing_Framework
$databricks_view_name = "V_PA105_EMAIL_MAX"
$SAP_View_Name = "CA_PA105_EMAIL_MAX"
$databricks_database_name="hr_original"
$sap_column_count="7"
$sap_row_count="15805"
$sap_duplicate_record_count="0"
$sap_null_column_name_list="PA105_PERNR_01"
$sap_null_column_value_list="0"
$sap_sum_column_name_list="COUNTER"
$sap_sum_column_value_list="15805"
$execution_time_of_sap_view="00.165110"
