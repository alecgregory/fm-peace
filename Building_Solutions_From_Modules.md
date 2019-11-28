# Building solution files from modules
1. Remove the whole <FileAccessCatalog> tag to prevent creating a damaged file being created
1. If a custom function with a matching name exists in the file, it will be overwritten, even if it is within the <AddAction> tage
1. Accounts and privilege sets should not be imported

