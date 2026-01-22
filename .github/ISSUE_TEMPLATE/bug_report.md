---
name: 🐛 Bug Report
about: Report a bug or unexpected behavior
title: '[BUG] '
labels: bug
assignees: ''
---

## Description

A clear description of what the bug is.

## Environment

- **RepliMap version**: (run `replimap --version`)
- **Python version**: (run `python --version`)
- **OS**: (e.g., macOS 14.2, Ubuntu 22.04, Windows 11)
- **AWS Region**: 
- **Resource types involved**: (e.g., EC2, RDS, Security Groups)

## Steps to Reproduce

1. Run `replimap scan --profile xxx --region xxx`
2. ...
3. See error

## Expected Behavior

What you expected to happen.

## Actual Behavior

What actually happened.

## Error Output

```
Paste any error messages here (remove sensitive info like account IDs)
```

## Generated Code (if applicable)

```hcl
# Paste relevant Terraform code that was generated incorrectly
```

## Additional Context

- [ ] This worked in a previous version (which version?)
- [ ] I have a valid license (`replimap license status`)
- [ ] My AWS credentials work (`aws sts get-caller-identity`)
- [ ] I've checked existing issues for duplicates
