---
api_specs:
- filename: unitrends-agents-api-openapi.yml
  format: yaml
  label: Unitrends Agents API
  slug: unitrends-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-agents-api-openapi.yml
- filename: unitrends-appliances-api-openapi.yml
  format: yaml
  label: Unitrends Appliances API
  slug: unitrends-appliances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-appliances-api-openapi.yml
- filename: unitrends-assets-api-openapi.yml
  format: yaml
  label: Unitrends Assets API
  slug: unitrends-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-assets-api-openapi.yml
- filename: unitrends-backupiqalerts-api-openapi.yml
  format: yaml
  label: Unitrends BackupIqAlerts API
  slug: unitrends-backupiqalerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-backupiqalerts-api-openapi.yml
- filename: unitrends-backups-api-openapi.yml
  format: yaml
  label: Unitrends Backups API
  slug: unitrends-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-backups-api-openapi.yml
- filename: unitrends-customers-api-openapi.yml
  format: yaml
  label: Unitrends Customers API
  slug: unitrends-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-customers-api-openapi.yml
- filename: unitrends-domains-api-openapi.yml
  format: yaml
  label: Unitrends Domains API
  slug: unitrends-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-domains-api-openapi.yml
- filename: unitrends-domainsentra-api-openapi.yml
  format: yaml
  label: Unitrends DomainsEntra API
  slug: unitrends-domainsentra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-domainsentra-api-openapi.yml
- filename: unitrends-domainsv2-api-openapi.yml
  format: yaml
  label: Unitrends DomainsV2 API
  slug: unitrends-domainsv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-domainsv2-api-openapi.yml
- filename: unitrends-domainusers-api-openapi.yml
  format: yaml
  label: Unitrends DomainUsers API
  slug: unitrends-domainusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-domainusers-api-openapi.yml
- filename: unitrends-domainusersv2-api-openapi.yml
  format: yaml
  label: Unitrends DomainUsersV2 API
  slug: unitrends-domainusersv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-domainusersv2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unitrends.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: backup.net
  spf: false
hosts:
- cert_expires: Sep  8 21:03:53 2026 GMT
  host: www.unitrends.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: apidoc-public-api.backup.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: public-api.backup.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unitrends Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unitrends, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unitrends
provider_slug: unitrends
slug: unitrends-domain-security
source_filename: unitrends-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unitrends.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: apidoc-public-api.backup.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: public-api.backup.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unitrends.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: backup.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/security/unitrends-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backup
- Disaster Recovery
- Data Protection
- BCDR
- Ransomware Protection
- MSP
- Endpoint Backup
---
