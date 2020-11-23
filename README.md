![Tests](https://github.com/vvish/install-gtest-gmock/workflows/Tests/badge.svg)

# install-gtest-gmock

The action installs the GoogleTest and GoogleMock frameworks onto the Linux-based GitHub Actions runners.

If the frameworks are not parts of the project they should be separately installed 
onto the system. This action performs this routine operation.

# Usage

```yaml
- uses: vvish/install-gtest-gmock@v1
  with:
    # Indicates if the GoogleMock framework should also be installed
    # Default: false
    gmock: ''
```

# Usage examples

Installs GoogleTest without GoogleMock

```yaml
- uses: vvish/install-gtest-gmock@v1
```

Installs GoogleTest with GoogleMock

```yaml
- uses: vvish/install-gtest-gmock@v1
  with:
    gmock: true
```

