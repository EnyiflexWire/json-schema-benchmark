# [`z-schema`](https://github.com/zaggino/z-schema) - test summary

# All validators fail this test

`some languages do not distinguish between different types of numeric value, a float is not an integer even without fractional part`

# [`z-schema`](https://github.com/zaggino/z-schema) failed tests

Some validators have deliberately chosen not to support parts of the spec. Go to the [`z-schema`](https://github.com/zaggino/z-schema) homepage to learn if
that is the case for these tests.

|test failed|reason
|-----------|------
`all integers are multiples of 0.5, if overflow is handled, valid if optional overflow handling is implemented`|Expected result: `true` but validator returned: `false`
`validation of IPv6 addresses, zone id is not a part of ipv6 address`|Expected result: `false` but validator returned: `true`
`validation of URIs, an invalid protocol-relative URI Reference`|Expected result: `false` but validator returned: `true`
`validation of URIs, an invalid relative URI Reference`|Expected result: `false` but validator returned: `true`
`validation of URIs, an invalid URI`|Expected result: `false` but validator returned: `true`
`validation of URIs, an invalid URI though valid URI reference`|Expected result: `false` but validator returned: `true`
`validation of URIs, an invalid URI with spaces`|Expected result: `false` but validator returned: `true`
`validation of URIs, an invalid URI with spaces and missing scheme`|Expected result: `false` but validator returned: `true`
`validation of URIs, an invalid URI with comma in scheme`|Expected result: `false` but validator returned: `true`
`Proper UTF-16 surrogate pair handling: pattern, matches empty`|Expected result: `true` but validator returned: `false`
`Proper UTF-16 surrogate pair handling: pattern, matches two`|Expected result: `true` but validator returned: `false`
`Proper UTF-16 surrogate pair handling: patternProperties, doesn't match two`|Expected result: `false` but validator returned: `true`
`Recursive references between schemas, valid tree`|Expected result: `true` but validator returned: `false`
`Location-independent identifier with absolute URI, match`|Expected result: `true` but validator returned: `false`
`Location-independent identifier with base URI change in subschema, match`|Expected result: `true` but validator returned: `false`
`naive replacement of $ref with its destination is not correct, match the enum exactly`|Expected result: `true` but validator returned: `false`
`ref within remote ref, ref within ref valid`|Expected result: `true` but validator returned: `false`
`base URI change - change folder, number is valid`|Expected result: `true` but validator returned: `false`
`base URI change - change folder in subschema, number is valid`|Expected result: `true` but validator returned: `false`
`root ref in remote ref, string is valid`|Expected result: `true` but validator returned: `false`

**All other tests passed**.

[back to benchmarks](https://github.com/ebdrup/json-schema-benchmark)