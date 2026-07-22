---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: claimsforce.com
  spf: true
hosts:
- cert_expires: Sep 30 19:36:43 2026 GMT
  host: www.claimsforce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Claimsforce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for claimsforce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: claimsforce
provider_slug: claimsforce
slug: claimsforce-domain-security
source_filename: claimsforce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.claimsforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:36:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: claimsforce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claimsforce/refs/heads/main/security/claimsforce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Claims Management
- Underwriting
- Risk Management
- SaaS
- Germany
---
