---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: korture.com
  spf: true
hosts:
- cert_expires: Feb  3 17:38:45 2027 GMT
  host: korture.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Korture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Korture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Korture
provider_slug: korture-com
slug: korture-com-domain-security
source_filename: korture-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: korture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 17:38:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: korture.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/korture-com/security/korture-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hiring
- Human Resources
- Behavioral Science
- Software-as-a-Service
- Talent Management
---
