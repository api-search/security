---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: formaportal.com
  spf: true
hosts:
- cert_expires: Jan 21 14:00:40 2027 GMT
  host: formaportal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FormaPortal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FormaPortal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FormaPortal
provider_slug: formaportal-com
slug: formaportal-com-domain-security
source_filename: formaportal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formaportal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 14:00:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: formaportal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/formaportal-com/security/formaportal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Portal
- GDPR
- No-Code
- Software-as-a-Service
---
