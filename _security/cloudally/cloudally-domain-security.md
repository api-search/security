---
api_specs:
- filename: cloudally-api-authorization-api-openapi.yml
  format: yaml
  label: CloudAlly API Authorization API
  slug: cloudally-api-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-api-authorization-api-openapi.yml
- filename: cloudally-backup-management-api-openapi.yml
  format: yaml
  label: CloudAlly Backup management API
  slug: cloudally-backup-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-backup-management-api-openapi.yml
- filename: cloudally-billing-management-api-openapi.yml
  format: yaml
  label: CloudAlly Billing management API
  slug: cloudally-billing-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-billing-management-api-openapi.yml
- filename: cloudally-distributor-backup-management-api-openapi.yml
  format: yaml
  label: CloudAlly Distributor Backup management API
  slug: cloudally-distributor-backup-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-distributor-backup-management-api-openapi.yml
- filename: cloudally-partner-portal-api-openapi.yml
  format: yaml
  label: CloudAlly Partner Portal API
  slug: cloudally-partner-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-partner-portal-api-openapi.yml
- filename: cloudally-reseller-backup-management-api-openapi.yml
  format: yaml
  label: CloudAlly Reseller Backup management API
  slug: cloudally-reseller-backup-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-reseller-backup-management-api-openapi.yml
- filename: cloudally-restore-download-api-openapi.yml
  format: yaml
  label: CloudAlly Restore & Download API
  slug: cloudally-restore-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-restore-download-api-openapi.yml
- filename: cloudally-user-management-api-openapi.yml
  format: yaml
  label: CloudAlly User management API
  slug: cloudally-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudally/openapi/cloudally-user-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudally.com
  spf: true
hosts:
- cert_expires: Sep 21 03:16:13 2026 GMT
  host: www.cloudally.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api.cloudally.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cloudally Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudAlly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CloudAlly
provider_slug: cloudally
slug: cloudally-domain-security
source_filename: cloudally-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudally.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:16:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cloudally.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cloudally.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cloudally/security/cloudally-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backup
- Box
- Data Protection
- Disaster Recovery
- Dropbox
- Google Workspace
- Microsoft 365
- OpenText
- SaaS Backup
- Salesforce
---
