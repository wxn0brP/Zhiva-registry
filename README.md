# Zhiva Registry

This repository serves as a central registry for Zhiva to manage verified and banned repositories.

## Structure

The registry is composed of two main files:

*   `verified.toml`: A list of repositories that have been manually verified.
*   `banned.toml`: A list of repositories that are banned due to malware, spam, or other issues.

## Formats

### verified.toml

To add a verified repository, append an entry with the following format:

```toml
[user/repo]
at = "YYYY-MM-DD"    # Date of verification
reason = "eg. manual verification" # Optional: Reason for verification
ref = "I-1 / P-1"    # Optional: Reference to an Issue or Pull Request
```

### banned.toml

To add a banned repository, append an entry with the following format:

```toml
[user/repo]
at = "YYYY-MM-DD"  # Date of banning
reason = "eg. malware / spam / etc" # Optional: Reason for banning
ref = "I-1 / P-1"    # Optional: Reference to an Issue or Pull Request
```

### References (`ref`)

The `ref` field can be used to link to a discussion in the [wxn0brP/Zhiva-registry](https://github.com/wxn0brP/Zhiva-registry) repository.

*   `I-1`: Refers to issue #1 (e.g., `https://github.com/wxn0brP/Zhiva-registry/issues/1`)
*   `P-1`: Refers to pull request #1 (e.g., `https://github.com/wxn0brP/Zhiva-registry/pull/1`)

## Contributing

To add or update an entry, please open a Pull Request. Ensure that your changes adhere to the specified TOML format.
