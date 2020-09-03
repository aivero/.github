# Aivero Pull Request

## Describe what this PR/MR is about, what does it add, fix or improve

----

## PR Review Checklist

These are based on the a variation of the boy-scout-rules.

Please make sure all of these are covered and ticked:

### Unit level code smells. 

Does the code smell on a unit (i.e. function) level. Confirm that **all** the functions are:

- [ ] Short (max 15 lines)
- [ ] Simple
- [ ] Have a simple interface, no more than 4 arguments. (Argue why you couldn't simplify the interface)

### Bad comments

Check the inline documentation:

- [ ] Inline documentation that is not updated or in-sync with the code
- [ ] Function- or module-level documentation that doesn't reflect the current workings of the fn/mod.
- [ ] Overly extensive documentation - could the documented code be replaced with a function?

### General smell of code

Check that there are none of the below:

- [ ] Code in comments
- [ ] Dead code
- [ ] Long identifiers
- [ ] Magic constants
- [ ] No badly handled exceptions. Or in Rust, preferably no .expect or .unwrap, unless we are 100% sure the code will no fail.

### Docs

- [ ] Is there a Changelog.[adoc, md, txt]?
- [ ] Does the changelog contain an entry documenting the changes of this MR and is the proposed version [SemVer](https://semver.org/) complient?

### Tests

There needs to be tests, how much and which is up to the reviewer to point out.

- [ ] Is there at least a single new test?
- [ ] Is the new code covered by unit tests?


----

test
