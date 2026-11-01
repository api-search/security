---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cymphony.io
  spf: true
hosts:
- cert_expires: Dec  4 22:54:30 2026 GMT
  host: cymphony.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cymphony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cymphony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cymphony
provider_slug: cymphony
slug: cymphony-domain-security
source_filename: cymphony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cymphony.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 22:54:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cymphony.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cymphony/security/cymphony-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- AI
- Workforce
- Identity
- Threat-Detection
- Enterprise
---
