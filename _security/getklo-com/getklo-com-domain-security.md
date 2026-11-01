---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getklo.com
  spf: false
hosts:
- cert_expires: Dec 18 08:16:35 2026 GMT
  host: getklo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getklo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for getklo-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: getklo-com
provider_slug: getklo-com
slug: getklo-com-domain-security
source_filename: getklo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getklo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 08:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getklo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getklo-com/security/getklo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video Editing
- AI
- Cloud Rendering
- Collaboration
- Marketing
---
