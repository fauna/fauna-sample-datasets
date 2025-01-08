# ByteMart e-commerce store schema creation files

This directory contains Fauna Schema Language (FSL) files to create the schema for a sample e-commerce store.

- [collections.fsl](./collections.fsl) - schema for the collections
- [functions.fsl](./functions.fsl) - schema for the user-defined functions (UDFs)
- [roles.fsl](./roles.fsl) - schema for the security roles

To create the schema, run the following command to stage the schema changes:

`fauna schema push --database=us/test_fauna`

To apply the schema changes, run the following command:

`fauna schema commit --database=us/test_fauna`

To add the sample data, run the following commands:

`cd ../data`

`fauna query -i ./demo-data.fql --database=us/test_fauna`