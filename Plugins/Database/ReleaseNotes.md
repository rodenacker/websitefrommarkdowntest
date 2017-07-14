# Release Notes for Database plugin

<a id="1_3_3_327"></a>
## 1.3.3.327
- Update MongoDb drivers.
- ExecuteSQL to use Transaction.
- BeginTransaction: Test all isolation levels.
- BeginTransaction: Added icon for Transaction object.
- ExecuteStoredProcedure to use Transaction.
- Update Linx plugin.
- Fix bug: Database connection wizard stays open after update.

<a id="1_2_3_303"></a>
## 1.2.3.303
- ConnectionEditor: Add Wizard to OLEDB type.
- Update Linx Plugin API.
- ExecuteSQL: Replace ConnectionString with ConnectionType and ConnectionString to give finer grained control over which drivers to use.
- Sort output tables.
- Fix bug: String as enumerable conversion error.
- ExecuteSQL (OLEDB): Fix locale settings related conversion issue with floating point valued sql parameters.
- Add BeginTransaction Function.

<a id="1_1_48_273"></a>
## 1.1.48.273
- Add DbBulkCopy function
- Update Linx plugin
- ExecuteStoredProcedure: Detect connection type when changing connection string
- ExecuteStoredProcedure: Fixed crash when setting connection string to a variable 
- UI changes

<a id="1_0_37_241"></a>
## 1.0.37.241
- Add ExecuteSQL function
- Add ExecuteStoredProcedure function
- Add MongoDBRead function
- Add MongoDBWrite function
