---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlas.health
  spf: true
hosts:
- cert_expires: Dec 26 23:12:08 2026 GMT
  host: atlas.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atlas Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Atlas
provider_slug: atlas-health
slug: atlas-health-domain-security
source_filename: atlas-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atlas.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:12:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atlas.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/atlas-health/security/atlas-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- AI
- PatientFinancing
- Platform
---
