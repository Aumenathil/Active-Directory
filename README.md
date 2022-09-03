# Active-Directory
# Enumerating ACLs, require PowerShell ISE. The following code block will enumerate all ACLs for a given directory. This is useful for tracking AD, tracking file access in your organization. An auditing tool.

$directory = Get-ChildItem ./
foreach ($item in $directory) {
  Get-Acl $item
 }
