---
description: ''
domains:
- caa:
  - ept-blinkhost-global-cyg2dhbfcwahdvf5.z01.azurefd.net.
  - mr-z01.tm-azurefd.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: blinkhost.me
  spf: false
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: blinkhost.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blinkhost Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for blinkhost-me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: blinkhost-me
provider_slug: blinkhost-me
slug: blinkhost-me-domain-security
source_filename: blinkhost-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blinkhost.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blinkhost.me\n  dnssec: true\n  caa:\n  - ept-blinkhost-global-cyg2dhbfcwahdvf5.z01.azurefd.net.\n  - mr-z01.tm-azurefd.net.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blinkhost-me/security/blinkhost-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Platform
- Full-Stack
- Developer Tools
- Edge Deployment
---
