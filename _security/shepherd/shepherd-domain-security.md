---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shepherdinsurance.com
  spf: false
hosts:
- cert_expires: Aug 22 09:46:16 2026 GMT
  host: shepherdinsurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shepherd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shepherd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Shepherd
provider_slug: shepherd
slug: shepherd-domain-security
source_filename: shepherd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shepherdinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 09:46:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shepherdinsurance.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shepherd/refs/heads/main/security/shepherd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Construction
- Commercial Insurance
- Underwriting
- Renewable Energy
---
