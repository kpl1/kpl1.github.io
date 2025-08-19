# Kibana

---


## Kibana Query Language (KQL)

**Range Queries:**
- To find documents with a field between two values:
`fieldname: [min_value TO max_value]`

- To find documents with a date field within a specific date range:
`date_field: [start_date TO end_date]`

**Wildcard Queries:**

- To find documents where a field starts with “prefix”:
`fieldname: prefix*`

- To find documents where a field contains “substring”:
`fieldname: *substring*`

**Fuzzy Queries:**

- To find documents with a field similar to “value” within a specific edit distance:
`fieldname: value~2`

**Nested Queries:**
- To search within a nested field:
`parent.nested_field: value`

**Boolean Queries:**

- To find documents that match multiple conditions:
`field1: value1 AND field2: value2`

- To find documents matching either of two conditions:
`field1: value1 OR field2: value2`

- To exclude documents matching a condition:
`NOT fieldname: value`

**Grouping Queries:**
- To create complex queries with multiple conditions:
`field1: value1 AND field2: value2`

**Exists and Missing Queries:**
- To find documents where a field exists:
`_exists_:fieldname`
- To find documents where a field is missing:
`_missing_:fieldname`

### Resources
- see official documentation [reference kql ](https://www.elastic.co/docs/reference/query-languages/kql?) 