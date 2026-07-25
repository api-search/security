---
api_specs:
- filename: druva-accounts-api-openapi.yml
  format: yaml
  label: Druva Accounts API
  slug: druva-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-accounts-api-openapi.yml
- filename: druva-authentication-api-openapi.yml
  format: yaml
  label: Druva Authentication API
  slug: druva-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-authentication-api-openapi.yml
- filename: druva-backups-api-openapi.yml
  format: yaml
  label: Druva Backups API
  slug: druva-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-backups-api-openapi.yml
- filename: druva-cyber-resilience-api-openapi.yml
  format: yaml
  label: Druva Cyber Resilience API
  slug: druva-cyber-resilience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cyber-resilience-api-openapi.yml
- filename: druva-policies-api-openapi.yml
  format: yaml
  label: Druva Policies API
  slug: druva-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-policies-api-openapi.yml
- filename: druva-reports-api-openapi.yml
  format: yaml
  label: Druva Reports API
  slug: druva-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-reports-api-openapi.yml
- filename: druva-schedules-api-openapi.yml
  format: yaml
  label: Druva Schedules API
  slug: druva-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-schedules-api-openapi.yml
- filename: druva-servers-api-openapi.yml
  format: yaml
  label: Druva Servers API
  slug: druva-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-servers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: druva.com
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: www.druva.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:09:39 2026 GMT
  host: developer.druva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 09:28:37 2026 GMT
  host: apis.druva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Druva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Druva, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Druva
provider_slug: druva
slug: druva-domain-security
source_filename: druva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.druva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.druva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:09:39 2026 GMT\n  hsts: null\n- host: apis.druva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 09:28:37 2026 GMT\n  hsts: null\ndomains:\n- domain: druva.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/security/druva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Backup
- Cyber Resilience
- Data Protection
- Disaster Recovery
- SaaS Backup
---
