# Todo

## Terms
- internal link count [functionality]
- incoming link count [functionality]

---- Tables ----

## Links
- [id] UUID? Integer
- [source_id] Indexable
- [target_id] Indexable (NULL)
- [URL] the used URL in the copy
- [type] (internal/external)

## Keywords
- [id] UUID? Integer
- [indexable_id] UUID? Integer
- [keyword] String
- [score] Integer
- [order] Integer

---- Tests -----

## Tests
Move all existing tests to `/tests/integrations/`.
Create `/tests/unittests/` for unittests.

---- Other -----

## Prefixing

Evaluate prefixing of global constants like `RUCKUSING_WORKING_BASE`

## UUID
- Can we use UUID?
- MySQL minimal version requirements?
- Autogenerated?
- Can the ORM handle these?

---- ORM does not support it out of the box, will need custom SQL implementation if we want to use the `UUID()` method of MySQL.

### prefix modules
* j4mie/paris
* j4mie/idiorm
* ruckusing/ruckusing-migrations

**Hacks implemented to make things work:**
- [Yoast_Model](https://github.com/Yoast/wordpress-seo/blob/yoast-meta/src/Yoast_Model.php#L7) to inject WordPress database table prefix the table names


# Final todo
Remove this file from the repository.