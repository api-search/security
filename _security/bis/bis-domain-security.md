---
api_specs:
- filename: bis-stats-api-latest.yaml
  format: yaml
  label: BIS Stats API
  slug: bis-stats-api
  spec_type: OpenAPI
  url: https://stats.bis.org/api-doc/v1/bis-stats-api-latest.yaml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "quovadisglobal.com"
  - 0 issue "swisssign.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bis.org
  spf: true
hosts:
- cert_expires: Sep 18 01:04:45 2026 GMT
  host: www.bis.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 01:02:47 2026 GMT
  host: stats.bis.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BIS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BIS
provider_slug: bis
slug: bis-domain-security
source_filename: bis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:04:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: stats.bis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:02:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bis.org\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"swisssign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bis/refs/heads/main/security/bis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Statistics
- Banking Data
- Derivatives
- Exchange Rates
- Central Bank
- SDMX
- Open Data
- International Finance
---
