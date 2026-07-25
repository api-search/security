---
api_specs:
- filename: eon-accounts-api-openapi.yml
  format: yaml
  label: Eon accounts API
  slug: eon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-accounts-api-openapi.yml
- filename: eon-actionapprovals-api-openapi.yml
  format: yaml
  label: Eon actionApprovals API
  slug: eon-actionapprovals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-actionapprovals-api-openapi.yml
- filename: eon-auth-api-openapi.yml
  format: yaml
  label: Eon auth API
  slug: eon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-auth-api-openapi.yml
- filename: eon-backuppolicies-api-openapi.yml
  format: yaml
  label: Eon backupPolicies API
  slug: eon-backuppolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-backuppolicies-api-openapi.yml
- filename: eon-backups-api-openapi.yml
  format: yaml
  label: Eon backups API
  slug: eon-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-backups-api-openapi.yml
- filename: eon-billing-api-openapi.yml
  format: yaml
  label: Eon billing API
  slug: eon-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-billing-api-openapi.yml
- filename: eon-dashboard-api-openapi.yml
  format: yaml
  label: Eon dashboard API
  slug: eon-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-dashboard-api-openapi.yml
- filename: eon-databasesnapshots-api-openapi.yml
  format: yaml
  label: Eon databaseSnapshots API
  slug: eon-databasesnapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-databasesnapshots-api-openapi.yml
- filename: eon-iam-api-openapi.yml
  format: yaml
  label: Eon iam API
  slug: eon-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-iam-api-openapi.yml
- filename: eon-jobs-api-openapi.yml
  format: yaml
  label: Eon jobs API
  slug: eon-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-jobs-api-openapi.yml
- filename: eon-resources-api-openapi.yml
  format: yaml
  label: Eon resources API
  slug: eon-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-resources-api-openapi.yml
- filename: eon-snapshots-api-openapi.yml
  format: yaml
  label: Eon snapshots API
  slug: eon-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-snapshots-api-openapi.yml
- filename: eon-vaults-api-openapi.yml
  format: yaml
  label: Eon vaults API
  slug: eon-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-vaults-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eon.io
  spf: true
hosts:
- cert_expires: Oct  6 12:24:09 2026 GMT
  host: eon.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eon
provider_slug: eon
slug: eon-domain-security
source_filename: eon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:24:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eon.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/security/eon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Backup
- Data Protection
- Disaster Recovery
- Ransomware Protection
- Backup
- Cloud Storage
- Data Lake
- Multi-Cloud
- Azure
- Google Cloud
---
