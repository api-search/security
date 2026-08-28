---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pocus.com
  spf: true
hosts:
- cert_expires: Sep 29 12:56:37 2026 GMT
  host: www.pocus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 17:20:22 2026 GMT
  host: docs.pocus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 03:25:51 2026 GMT
  host: api.pocus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pocus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pocus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pocus
provider_slug: pocus
slug: pocus-domain-security
source_filename: pocus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pocus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:56:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pocus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 17:20:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pocus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 03:25:51 2026 GMT\n  hsts: null\ndomains:\n- domain: pocus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocus/refs/heads/main/security/pocus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales Intelligence
- Product-Led Sales
- Revenue Operations
- Go-To-Market
- Data Enrichment
- CRM
- Artificial Intelligence
- GraphQL
---
