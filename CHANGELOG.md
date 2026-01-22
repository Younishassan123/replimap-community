# Changelog

All notable changes to RepliMap will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [0.3.2] - 2026-01-20

### Fixed
- **EC2 `root_block_device` handling** — Fixed attribute mapping that could trigger unintended instance replacement. Read-only fields like `device_name` are now properly filtered.
- **AWS system tag filtering** — All 21 resource templates now filter `aws:*` prefix tags to prevent API rejection errors.
- **Security Group circular dependencies** — Automatic splitting into separate `aws_security_group_rule` resources.
- **ASG Target Group references** — Proper variable fallback (`var.unmapped_tg_*`) for missing target groups.
- **S3 bucket name length** — Smart handling for buckets exceeding 63 character limit.
- **ElastiCache Redis version format** — Strips patch version (6.2.6 → 6.2) as required by Terraform provider.

### Added
- **Blast Radius Analyzer** *(Pro)* — Analyze deletion impact before running `terraform destroy`
- **Cost Estimator** *(Pro)* — Monthly cost estimation with optimization recommendations
- **Interactive Graph Visualization** — D3.js-powered infrastructure topology map

---

## [0.3.0] - 2026-01-15

### Added
- CloudFormation output support *(Solo+)*
- Pulumi output support *(Pro+)*
- Makefile generation for Terraform workflows
- Local scan caching with `--cache` flag

### Changed
- License key format updated to `RM-XXXX-XXXX-XXXX-XXXX`

---

## [0.2.0] - 2026-01-01

### Added
- **Drift Detection** *(Pro)* — Compare actual AWS state with Terraform code
- 24 AWS resource type scanners
- Graph-based dependency resolution using NetworkX

---

## [0.1.0] - 2025-12-15

### Added
- Initial release
- Core scanners: VPC, Subnet, Security Group, EC2, RDS, S3
- Terraform HCL output
- Basic dependency tracking

---

For detailed release notes, visit [replimap.com/changelog](https://replimap.com/changelog)
