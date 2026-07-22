---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gilion.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: www.gilion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gilion Formerly Ark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gilion (formerly ArK), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gilion (formerly ArK)
provider_slug: gilion-formerly-ark
slug: gilion-formerly-ark-domain-security
source_filename: gilion-formerly-ark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gilion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gilion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gilion-formerly-ark/refs/heads/main/security/gilion-formerly-ark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- Growth Financing
- Venture Debt
- Artificial Intelligence
- Investment
- SaaS
---
