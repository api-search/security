---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: shield.com
  spf: true
hosts:
- cert_expires: Jan 24 14:51:27 2027 GMT
  host: shield.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SHIELD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SHIELD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SHIELD
provider_slug: shield-com
slug: shield-com-domain-security
source_filename: shield-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 14:51:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shield.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/shield-com/security/shield-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fraud Prevention
- Device-First
- Artificial Intelligence
- Detection
---
