---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hnicorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hearthnhome.com
  spf: true
hosts:
- cert_expires: Nov 26 13:01:13 2026 GMT
  host: www.hnicorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 09:09:31 2026 GMT
  host: hearthnhome.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Hni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HNI Corporation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HNI Corporation
provider_slug: hni
slug: hni-domain-security
source_filename: hni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hnicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 13:01:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hearthnhome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 09:09:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hnicorp.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hearthnhome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hni/refs/heads/main/security/hni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
- Manufacturing
- Office Furniture
- Workplace
- Building Products
- Hearth
- Retail
- E-Commerce
- Agentic Commerce
- MCP
---
