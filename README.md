# Analysis-template

A simple starting point for a new project.

Directory structure

    -|
     |-config       * configuration files
     |-data         * working data
     |-data-raw     * raw data (should not be modified by code)
     |-outputs      * outputs (e.g. tables, figures, documents)
     |-src          * code


For the example code to work off the shelf, you will need to place an `.RData` file containing data as a `ccRecord` class object named `ccd` into the `data-raw` directory. The file should be named `anon_ccd_k_5.RData`.

Files for a minimal working example

    -|
     |-config       
        |- data_fields.yaml     * field configuration
     |-data         
     |-data-raw     
        |- anon_ccd_k_5.RData   * contains `ccd` object
     |-outputs      
     |-src          
        |- raw2working.R        * clean and validate `ccRecord` object
        |- derive.R             * derive secondary variables
        |- working_inspect.R    * simple inspection of data

There are two branches in this repository.

The **master** branch contains a very minimal working example with just a handful of fields from the raw data. The **try-sofa** branch pulls in some extra fields and then derives the SOFA score.

