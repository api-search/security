---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gravito.net
  spf: true
hosts:
- cert_expires: Dec 16 01:04:41 2026 GMT
  host: gravito.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gravito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravito, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gravito
provider_slug: gravito
slug: gravito-domain-security
source_filename: gravito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gravito.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 01:04:41 2026 GMT\n  hsts: false\ndomains:\n- domain: gravito.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gravito/security/gravito-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consent Management
- Data Platform
- Traffic Quality
- First-Party Data
- Privacy
---
