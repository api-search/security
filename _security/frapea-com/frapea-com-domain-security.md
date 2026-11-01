---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: frapea.com
  spf: true
hosts:
- cert_expires: Jan 18 01:57:40 2027 GMT
  host: frapea.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Frapea Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for frapea-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: frapea-com
provider_slug: frapea-com
slug: frapea-com-domain-security
source_filename: frapea-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frapea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 01:57:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: frapea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/frapea-com/security/frapea-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video Editing
- AI
- Browser-based
- No-install
- Creative Tools
---
