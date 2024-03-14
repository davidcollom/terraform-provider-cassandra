# cassandra_table

Creates a table.

## Example Usage

```hcl
resource "cassandra_table" "table" {
  name     = "my_table"
  keyspace = "my-keyspace"
  row_keys = ["Name", "Email"]
}
```

## Argument Reference

- `name` - Name of the table. Must contain between 1 and 256 characters.

- `keyspace` - Keyspace in which to create the table within.

- `row_keys` - List of Row Keys

- `range_keys` - List of row keys to use for ranges/partitioning.
