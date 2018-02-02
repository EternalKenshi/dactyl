# Dactyl Tests

The following files test different parts of Dactyl:

- [testdactyl.py](./testdactyl.py) - Integration tests
- [testdactylbuild.py](./testdactylbuild.py) - Unit tests for `dactyl_build.py`

# Running Integration Tests

Integration tests should be run from the "examples" directory using the following command.

```
python3 ../tests/testdactyl.py
```

These tests should ideally be run prior to any new commit to validate Dactyl's core functions remain intact.

# Running Unit Tests

Unit tests should be run from the "tests" directory, to ensure that test config files and mocks are loaded correctly, using the following command.

```
python3 testdactylbuild.py
```

These tests are primarily used to clearly define the behavior of functions defined in dactyl_build.py, and should ideally be run whenever code is refactored to ensure that behavior remains consistent.