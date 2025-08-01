To run weekly updates, downloand the pyscript and copy the launchd plist script onto your MacOS terminal.

For the plist script. make sure to change the YOUR_USERNAME and PATH_TO_PYSCRIPT with your actual macOS username and full path to your pyscript file

The launchd plist script will:

- Pull pitch data from the past week

- Append it to your PostgreSQL database (if DATABASE_URL is correctly set in your .env)

- Append info to your etl_output.log and etl_dates.log

- The logs will accumulate each day — not be overwritten


You will also need to create a .env file in the same path as the pyscript with the following variable:

DATABASE_URL = postgresql://username:password@host:port/dbname

where you'll replace the following to connect to you postgreSQL server:

- username
- password
- host
- port
- dbname
