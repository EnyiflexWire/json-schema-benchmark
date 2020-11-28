# [`ajv`](https://github.com/ajv-validator/ajv) - test summary

# All validators fail this test

`some languages do not distinguish between different types of numeric value, a float is not an integer even without fractional part`

# [`ajv`](https://github.com/ajv-validator/ajv) failed tests

Some validators have deliberately chosen not to support parts of the spec. Go to the [`ajv`](https://github.com/ajv-validator/ajv) homepage to learn if
that is the case for these tests.

|test failed|reason
|-----------|------
`all integers are multiples of 0.5, if overflow is handled, valid if optional overflow handling is implemented`|Expected result: `true` but validator returned: `false`
`validation of e-mail addresses, dot before local part is not valid`|Expected result: `false` but validator returned: `true`
`validation of e-mail addresses, dot after local part is not valid`|Expected result: `false` but validator returned: `true`
`validation of e-mail addresses, two subsequent dots inside local part are not valid`|Expected result: `false` but validator returned: `true`
`validation of IPv6 addresses, leading whitespace is invalid`|Expected result: `false` but validator returned: `true`
`validation of IPv6 addresses, trailing whitespace is invalid`|Expected result: `false` but validator returned: `true`
`validation of IPv6 addresses, zone id is not a part of ipv6 address`|Expected result: `false` but validator returned: `true`
`Proper UTF-16 surrogate pair handling: pattern, matches empty`|Expected result: `true` but validator returned: `false`
`Proper UTF-16 surrogate pair handling: pattern, matches two`|Expected result: `true` but validator returned: `false`
`Proper UTF-16 surrogate pair handling: patternProperties, doesn't match two`|Expected result: `false` but validator returned: `true`
`Location-independent identifier, match`|The schema failed to load(`schema is invalid: data.definitions['A'].id should match format "uri"`)
`Location-independent identifier, mismatch`|The schema failed to load(`schema is invalid: data.definitions['A'].id should match format "uri"`)
`Location-independent identifier with base URI change in subschema, match`|The schema failed to load(`schema is invalid: data.definitions['A'].id should match format "uri"`)
`Location-independent identifier with base URI change in subschema, mismatch`|The schema failed to load(`schema is invalid: data.definitions['A'].id should match format "uri"`)
`base URI change, base URI change ref valid`|The schema failed to load(`schema is invalid: data.items.id should match format "uri", data.items should be array, data.items should match some schema in anyOf`)
`base URI change, base URI change ref invalid`|The schema failed to load(`schema is invalid: data.items.id should match format "uri", data.items should be array, data.items should match some schema in anyOf`)
`base URI change - change folder, number is valid`|The schema failed to load(`schema is invalid: data.definitions['baz'].id should match format "uri"`)
`base URI change - change folder, string is invalid`|The schema failed to load(`schema is invalid: data.definitions['baz'].id should match format "uri"`)
`base URI change - change folder in subschema, number is valid`|The schema failed to load(`schema is invalid: data.definitions['baz'].id should match format "uri"`)
`base URI change - change folder in subschema, string is invalid`|The schema failed to load(`schema is invalid: data.definitions['baz'].id should match format "uri"`)

**All other tests passed**.

[back to benchmarks](https://github.com/ebdrup/json-schema-benchmark)