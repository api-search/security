---
api_specs:
- filename: harvest-openapi.yml
  format: yaml
  label: Harvest API v2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harvest/refs/heads/main/openapi/harvest-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:systems@getharvest.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getharvest.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:systems@getharvest.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: harvestapp.com
  spf: true
hosts:
- cert_expires: Sep 10 03:41:04 2026 GMT
  host: www.getharvest.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:10:37 2026 GMT
  host: help.getharvest.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 19:13:42 2026 GMT
  host: api.harvestapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harvest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harvest, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Harvest
provider_slug: harvest
slug: harvest-domain-security
source_filename: harvest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getharvest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:41:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.getharvest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:10:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.harvestapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 19:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getharvest.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:systems@getharvest.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: harvestapp.com\n  dnssec: false\n  caa:\n  - 0 issuewild\
  \ \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:systems@getharvest.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harvest/refs/heads/main/security/harvest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Time Tracking
- Project Management
- Invoicing
- Expense Tracking
- Timesheets
- Professional Services
---
