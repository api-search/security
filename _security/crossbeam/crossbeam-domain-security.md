---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:eyebeams@crossbeam.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crossbeam.com
  spf: true
hosts:
- cert_expires: Oct 14 13:35:39 2026 GMT
  host: www.crossbeam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:00:10 2026 GMT
  host: developers.crossbeam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: api.crossbeam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Crossbeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossbeam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Crossbeam
provider_slug: crossbeam
slug: crossbeam-domain-security
source_filename: crossbeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossbeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:35:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.crossbeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.crossbeam.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crossbeam.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:eyebeams@crossbeam.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossbeam/refs/heads/main/security/crossbeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ecosystem-Led Growth
- Partnerships
- Account Mapping
- Co-Selling
- Data Collaboration
- Sales Intelligence
- CRM
- Webhooks
- MCP
---
