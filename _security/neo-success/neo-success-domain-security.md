---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neomoney.com
  spf: true
hosts:
- cert_expires: Jan 25 18:20:24 2027 GMT
  host: neomoney.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neo Success Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NEO Success, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NEO Success
provider_slug: neo-success
slug: neo-success-domain-security
source_filename: neo-success-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neomoney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 18:20:24 2027 GMT\n  hsts: null\ndomains:\n- domain: neomoney.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neo-success/refs/heads/main/security/neo-success-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Personal Finance
- Money Management
- Neobank
- Thailand
- Defunct
---
