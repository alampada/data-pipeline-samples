# DynamoDB from CSV import

## About the sample

The pipeline definition is used to import DynamoDB data from a CSV format.

## Running the pipeline

Example DynamoDB table with keys: id

User needs to provide:

1. Input S3 folder: The source S3 folder prefix from which the CSV data is to be imported.
2. DynamoDB table name: The name of the target dynamo table.
3. S3 Column Mappings: Comma seperated column definitions. For example, customer_id string, income string, demographics string, financial string.
4. Dynamodb Column Mappings: Comma seperated column definitions. For example, customer_id string, income string, demographics string, financial string
5. S3 to DynamoDB Column Mapping: Comma separated mapping from S3 to DynamoDB for e.g. customer_id:customer_id,income:income,demographics:demographics,financial:financial. Please take care of not using spaces in between the commas.
6. Log Uri: S3 log path to capture the pipeline logs.
