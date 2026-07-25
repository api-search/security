---
api_specs:
- filename: aws-backup-backup-jobs-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Jobs API
  slug: aws-backup-backup-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-jobs-api-openapi.yml
- filename: aws-backup-backup-plans-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Plans API
  slug: aws-backup-backup-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-plans-api-openapi.yml
- filename: aws-backup-backup-selections-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Selections API
  slug: aws-backup-backup-selections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-selections-api-openapi.yml
- filename: aws-backup-backup-vaults-api-openapi.yml
  format: yaml
  label: AWS Backup Backup Vaults API
  slug: aws-backup-backup-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-backup-vaults-api-openapi.yml
- filename: aws-backup-copy-jobs-api-openapi.yml
  format: yaml
  label: AWS Backup Copy Jobs API
  slug: aws-backup-copy-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-copy-jobs-api-openapi.yml
- filename: aws-backup-frameworks-api-openapi.yml
  format: yaml
  label: AWS Backup Frameworks API
  slug: aws-backup-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-frameworks-api-openapi.yml
- filename: aws-backup-recovery-points-api-openapi.yml
  format: yaml
  label: AWS Backup Recovery Points API
  slug: aws-backup-recovery-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-recovery-points-api-openapi.yml
- filename: aws-backup-report-plans-api-openapi.yml
  format: yaml
  label: AWS Backup Report Plans API
  slug: aws-backup-report-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-report-plans-api-openapi.yml
- filename: aws-backup-restore-jobs-api-openapi.yml
  format: yaml
  label: AWS Backup Restore Jobs API
  slug: aws-backup-restore-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-restore-jobs-api-openapi.yml
- filename: aws-backup-tags-api-openapi.yml
  format: yaml
  label: AWS Backup Tags API
  slug: aws-backup-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/openapi/aws-backup-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: backup.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aws Backup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS Backup, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS Backup
provider_slug: aws-backup
slug: aws-backup-domain-security
source_filename: aws-backup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: backup.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-backup/refs/heads/main/security/aws-backup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backup
- Data Protection
- Disaster Recovery
- Managed Service
- Compliance
---
