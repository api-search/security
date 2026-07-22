---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: freestyle.vc
  spf: false
hosts:
- cert_expires: Aug 27 22:08:12 2026 GMT
  host: freestyle.vc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freestyle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freestyle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Freestyle
provider_slug: freestyle
slug: freestyle-domain-security
source_filename: freestyle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freestyle.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:08:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freestyle.vc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freestyle/refs/heads/main/security/freestyle-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Venture Capital
- Investment
- Startups
- Seed Stage
- Artificial Intelligence
---
