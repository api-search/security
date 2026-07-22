---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sxd.ai
  spf: false
hosts:
- cert_expires: Oct 15 21:48:19 2026 GMT
  host: sxd.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sxd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SXD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SXD
provider_slug: sxd
slug: sxd-domain-security
source_filename: sxd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sxd.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sxd.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sxd/refs/heads/main/security/sxd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise Saas
- Fashion
- Sustainability
- Artificial Intelligence
- Design
- Apparel
- Manufacturing
---
