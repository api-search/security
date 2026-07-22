---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: true
  domain: metaphor.io
  spf: true
hosts:
- cert_expires: Oct 17 02:03:57 2026 GMT
  host: metaphor.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metaphor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metaphor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Metaphor
provider_slug: metaphor
slug: metaphor-domain-security
source_filename: metaphor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metaphor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:03:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: metaphor.io\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metaphor/refs/heads/main/security/metaphor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Data Analytics
- Metadata
- Data Catalog
- Data Governance
- Data Lineage
- Active Metadata
---
