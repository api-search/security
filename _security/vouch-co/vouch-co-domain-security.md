---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vouch.us
  spf: true
hosts:
- cert_expires: Sep  3 01:42:44 2026 GMT
  host: www.vouch.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vouch Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vouch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vouch
provider_slug: vouch-co
slug: vouch-co-domain-security
source_filename: vouch-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vouch.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 01:42:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vouch.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vouch-co/refs/heads/main/security/vouch-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Business Insurance
- Commercial Insurance
- Insurtech
- Startup Insurance
- Directors And Officers
- Errors And Omissions
- Cyber Insurance
- Employment Practices Liability
- General Liability
- Embedded Insurance
- Risk Management
- Brokerage
- Underwriting
- Venture Ecosystem
---
