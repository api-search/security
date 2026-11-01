---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: webcapture.io
  spf: true
hosts:
- cert_expires: Dec  1 04:38:10 2026 GMT
  host: webcapture.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Webcapture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for webcapture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: webcapture
provider_slug: webcapture
slug: webcapture-domain-security
source_filename: webcapture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webcapture.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 04:38:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: webcapture.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/webcapture/security/webcapture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- WebCapture
- PDF
- API
- SaaS
- Automation
---
