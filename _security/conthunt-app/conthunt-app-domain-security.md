---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conthunt.app
  spf: true
hosts:
- cert_expires: Dec  8 00:39:30 2026 GMT
  host: conthunt.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ContHunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ContHunt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ContHunt
provider_slug: conthunt-app
slug: conthunt-app-domain-security
source_filename: conthunt-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conthunt.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 00:39:30 2026 GMT\n  hsts: false\ndomains:\n- domain: conthunt.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/conthunt-app/security/conthunt-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Artificial Intelligence
- Analytics
- Marketing
- Social Media
---
