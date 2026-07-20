---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autonomic.ai
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: autonomic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: developer.autonomic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autonomic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autonomic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Autonomic
provider_slug: autonomic
slug: autonomic-domain-security
source_filename: autonomic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autonomic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: developer.autonomic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: autonomic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autonomic/refs/heads/main/security/autonomic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure
- Automotive
- Connected Vehicles
- Mobility
- Cloud
- IoT
---
