---
api_specs:
- filename: sisense-rest-api-openapi.yml
  format: yaml
  label: Sisense REST API v1
  slug: rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sisense/refs/heads/main/openapi/sisense-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sisense.com
  spf: true
hosts:
- cert_expires: Aug 12 10:28:42 2026 GMT
  host: www.sisense.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:17:18 2026 GMT
  host: developer.sisense.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 02:10:46 2026 GMT
  host: dtdocs.sisense.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sisense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sisense, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sisense
provider_slug: sisense
slug: sisense-domain-security
source_filename: sisense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sisense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 10:28:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sisense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:17:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dtdocs.sisense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 02:10:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sisense.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sisense/refs/heads/main/security/sisense-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Models
- Embedded Analytics
---
