---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dailystudio.app
  spf: false
hosts:
- cert_expires: Dec 16 15:14:22 2026 GMT
  host: dailystudio.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dailystudio App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daily Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Daily Studio
provider_slug: dailystudio-app
slug: dailystudio-app-domain-security
source_filename: dailystudio-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dailystudio.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:14:22 2026 GMT\n  hsts: false\ndomains:\n- domain: dailystudio.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dailystudio-app/security/dailystudio-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software-as-a-Service
- Video
- Content Creation
- Teleprompter
- Artificial Intelligence
---
