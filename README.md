# Zhiva Registry

This repository serves as a central registry for Zhiva to manage verified and banned repositories.

## Structure

The registry is composed of two main files:

*   `verified.txt`: A list of repositories that have been manually verified.
*   `banned.txt`: A list of repositories that are banned due to malware, spam, or other issues.

## Formats

The format for both `verified.txt` and `banned.txt` is a simple line-by-line list. Each line can be one of the following:

- `user/repo`
- `user/repo#I-id`
- `user/repo#P-id`

### References

*   `I-1`: Refers to issue #1 (e.g., `https://github.com/wxn0brP/Zhiva-registry/issues/1`)
*   `P-1`: Refers to pull request #1 (e.g., `https://github.com/wxn0brP/Zhiva-registry/pull/1`)

## Contributing

To add or update an entry, please open a Pull Request.

