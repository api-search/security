---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veroscribe.com
  spf: true
hosts:
- cert_expires: Jan 24 20:20:32 2027 GMT
  host: www.veroscribe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vero
provider_slug: veroscribe-com
slug: veroscribe-com-domain-security
source_filename: veroscribe-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veroscribe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 20:20:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: veroscribe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/veroscribe-com/security/veroscribe-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Medical
- Scribe
- Clinical Documentation
- Healthcare
---
