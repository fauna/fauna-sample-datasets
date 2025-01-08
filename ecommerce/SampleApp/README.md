# E-commerce sample app store schema creation files

This directory contains Fauna Schema Language (FSL) files to create the schema for a sample e-commerce store.

- [collections.fsl](./collections.fsl) - schema for the collections
- [functions.fsl](./functions.fsl) - schema for the user-defined functions (UDFs)
- [roles.fsl](./roles.fsl) - schema for the security roles

To create the schema and commit those changes, run the following commands:
- `cd schema`
- `fauna schema push --database=us/test_fauna`
- `fauna schema commit --database=us/test_fauna`

To add the sample data, run the following commands:

- `cd ../data`
- `fauna query -i ./demo-data.fql --database=us/test_fauna`