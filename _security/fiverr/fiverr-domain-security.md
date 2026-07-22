---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fiverr.com
  spf: true
hosts:
- cert_expires: Oct  9 12:14:06 2026 GMT
  host: www.fiverr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fiverr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiverr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fiverr
provider_slug: fiverr
slug: fiverr-domain-security
source_filename: fiverr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fiverr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 12:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fiverr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiverr/refs/heads/main/security/fiverr-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Freelance
- Marketplace
- Gig Economy
- Digital Services
---
