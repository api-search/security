---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: helloverify.com
  spf: true
hosts:
- cert_expires: Oct  1 04:42:22 2026 GMT
  host: www.helloverify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Helloverify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HelloVerify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HelloVerify
provider_slug: helloverify
slug: helloverify-domain-security
source_filename: helloverify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helloverify.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 04:42:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helloverify.com\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helloverify/refs/heads/main/security/helloverify-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Background Verification
- Employee Screening
- Identity Verification
- KYC
- Primary Source Verification
- Compliance
- HR Tech
---
