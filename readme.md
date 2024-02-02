This script will accept a parameter input log_directory: a directory where 
application will write logs.

The script will check whether the parameter value is a directory name that 
doesn't exist and will create the directory, if it does exist, it sets 
the env var LOG_DIR to the directory's absolute path before running the 
application, so the application can read the LOG_DIR environment variable 
and write its logs there.

Note:

Check the app.log file in the provided LOG_DIR directory. This is what the output of running the application must look like: node-app-output.png

Make file executable with:

    chmod +x extended_install_and_run_with_log.sh

Execute it with the desired log directory as a parameter:

    ./extended_install_and_run_with_log.sh log_ID
