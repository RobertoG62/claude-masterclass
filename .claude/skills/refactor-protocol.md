# Refactor Protocol - Safe Code Changes

## Step-by-Step Guide for Safe Refactoring

### Phase 1: Preparation
1. **Read the target code** - Never modify code you haven't read
2. **Understand the context** - Check how the code is used elsewhere
3. **Identify dependencies** - Find all files that import/reference this code
4. **Check for tests** - Locate existing test coverage

### Phase 2: Analysis
1. **Document current behavior** - Note what the code does now
2. **Identify the change scope** - Determine exactly what needs to change
3. **Plan the minimal change** - Avoid scope creep and over-engineering
4. **Consider edge cases** - Think about error handling and boundaries

### Phase 3: Implementation
1. **Make atomic changes** - One logical change at a time
2. **Preserve interfaces** - Don't break external contracts unless necessary
3. **Update call sites** - Modify all places that use the changed code
4. **Keep backwards compatibility** - Only when explicitly required

### Phase 4: Verification
1. **Run existing tests** - Ensure nothing broke
2. **Test the new behavior** - Verify the change works as intended
3. **Check for regressions** - Look for unintended side effects
4. **Review the diff** - Confirm only intended changes were made

### Phase 5: Cleanup
1. **Remove dead code** - Delete unused functions/variables completely
2. **Update documentation** - Only if existing docs need correction
3. **Commit atomically** - One logical change per commit
4. **Use descriptive messages** - Explain "why" not just "what"

## Safety Checklist

- [ ] Read all files before modifying
- [ ] Understood the purpose of existing code
- [ ] Identified all affected files
- [ ] Made minimal necessary changes
- [ ] Tested the changes work
- [ ] No new warnings or errors introduced
- [ ] Diff contains only intended changes
