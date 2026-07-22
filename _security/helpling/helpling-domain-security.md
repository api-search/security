---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: helpling.de
  spf: true
hosts:
- cert_expires: Oct  5 10:16:52 2026 GMT
  host: www.helpling.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Helpling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helpling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Helpling
provider_slug: helpling
slug: helpling-domain-security
source_filename: helpling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helpling.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 10:16:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helpling.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpling/refs/heads/main/security/helpling-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Cleaning Services
- Home Services
- Marketplace
- On-Demand
- Gig Economy
- Consumer
- Germany
---
