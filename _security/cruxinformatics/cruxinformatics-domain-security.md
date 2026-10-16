---
api_specs:
- filename: cruxinformatics-openapi-generated.yml
  format: yaml
  label: Cruxinformatics API
  slug: cruxinformatics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruxinformatics/refs/heads/main/openapi/_ae-authored/cruxinformatics-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cruxdata.com
  spf: true
hosts:
- cert_expires: Dec 28 23:16:35 2026 GMT
  host: www.cruxdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cruxinformatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cruxinformatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cruxinformatics
provider_slug: cruxinformatics
slug: cruxinformatics-domain-security
source_filename: cruxinformatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cruxdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cruxdata.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cruxinformatics/refs/heads/main/security/cruxinformatics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- AI
- Financial Services
- Managed Service
- Self-Service
---
