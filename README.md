# Install-Kontrol
An action used to install Runtime Verification Inc Kontrol. 

# What's New
please refer to the [release page](https://github.com/runtimeverification/install-kontrol/releases) for the latest notes.

# Usage
Kontrol Release Page: [Kontrol Releases](https://github.com/runtimeverification/kontrol/releases)
<!-- start usage -->
```yaml
- uses: runtimeverification/install-kontrol@v1
  with: 
    # Set version of Kontrol to use. Format of versions are in the format of 'v0.0.0'.
    # Otherwise, the latest version will be used.
    # For a list of available releases please see the above link to Kontrol Releases Page
    # Default: 'latest'
    version: ''
```
<!-- end usage -->


#  Scenarios

- [Use the latest version of Kontrol](#use-the-latest-version-of-kontrol)
- [Use a specific version of Kontrol](#use-a-specific-version-of-kontrol)

## Use the latest version of Kontrol
```yaml
- uses: runtimeverification/install-kontrol@v1

- run: kontrol version
```
or 
```yaml
- uses: runtimeverification/install-kontrol@v1
  with: 
    version: 'latest'
- run: kontrol version
```

## Use a specific version of Kontrol
```yaml
- uses: runtimeverification/install-kontrol@v1
  with: 
    version: 'v0.1.229'

- run: kontrol version
```

# License

The scripts and documentation in this project are released under the [MIT License](LICENSE)