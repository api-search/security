---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: homegp.asia
  spf: true
hosts:
- cert_expires: Oct 15 02:06:45 2026 GMT
  host: homegp.asia
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homegp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeGP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HomeGP
provider_slug: homegp
slug: homegp-domain-security
source_filename: homegp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homegp.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:06:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: homegp.asia\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homegp/refs/heads/main/security/homegp-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Home Care
- House Calls
- Nursing
- Physiotherapy
- Caregivers
- Telehealth
- Malaysia
- Marketplace
---
