---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: propmatic.co
  spf: true
hosts:
- cert_expires: Oct 11 10:14:54 2026 GMT
  host: propmatic.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propmatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propmatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Propmatic
provider_slug: propmatic
slug: propmatic-domain-security
source_filename: propmatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: propmatic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:14:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: propmatic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propmatic/refs/heads/main/security/propmatic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Proptech
- Real Estate
- Leasing
- Multifamily
- Artificial Intelligence
- MCP
---
