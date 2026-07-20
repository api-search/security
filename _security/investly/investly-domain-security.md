---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: investly.co
  spf: true
hosts:
- cert_expires: Sep 19 04:57:22 2026 GMT
  host: www.investly.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.investly.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Investly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Investly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Investly
provider_slug: investly
slug: investly-domain-security
source_filename: investly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.investly.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:57:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.investly.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: investly.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/investly/refs/heads/main/security/investly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Invoice Finance
- Invoice Discounting
- Lending
- Working Capital
- SME Finance
- Marketplace
- Estonia
- United Kingdom
---
