/*
===================================================================================================================
-- Create Database "Datawarehouse"
===================================================================================================================
Script Purpose;
     This script creates new database named 'Datawarehouse' if the batabase already exists the will check and drop
     the existing the database and recreate a new batabase. further, this script additionally set-up three schemas
     within the database named - "bronze", "silver", and "gold"
WARNING;
     Running the script will delet all the data exists in database - Datawarehouse if exists. ALL DATA WILL IN THE 
     DATABASE PERMANENTLY DELETED. Proceed with caution and ensure you have backup before proceeding with the script.

*/
USE master;
GO

--Drop and recreate the 'Datawarehouse' database
IF EXISTS (SELECT 1 FROM sys.databases WHERE name = 'DataWarehouse')
BEGIN
    ALTER DATABASE Datawarehouse SET SINGLE_USER WITH ROLLBACK IMMEDIATE;
    DROP DATABASE DataWarehouse;
END;
GO

-- Crete new database "Datawarehouse"
CREATE DATABASE DataWarehouse;
GO

USE DataWarehouse;
GO

-- Create schemas:

CREATE SCHEMA bronze;
GO

CREATE SCHEMA silver;
GO

CREATE SCHEMA gold;
