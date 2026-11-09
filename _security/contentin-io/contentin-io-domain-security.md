---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contentin.io
  spf: true
hosts:
- cert_expires: Dec 20 20:50:17 2026 GMT
  host: contentin.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contentin Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ContentIn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ContentIn
provider_slug: contentin-io
slug: contentin-io-domain-security
source_filename: contentin-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contentin.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 20:50:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: contentin.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/contentin-io/security/contentin-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LinkedIn
- Ghostwriter
- Content Creation
- Software-as-a-Service
- Company
---
