---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: izotope.com
  spf: true
hosts:
- cert_expires: Sep 17 22:05:02 2026 GMT
  host: www.izotope.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Izotope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iZotope, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iZotope
provider_slug: izotope
slug: izotope-domain-security
source_filename: izotope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.izotope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:05:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: izotope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/izotope/refs/heads/main/security/izotope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Audio
- Audio Software
- Music Production
- Mixing
- Mastering
- Audio Restoration
- Audio Repair
- Post Production
- Plugins
- VST
- AudioUnit
- AAX
- DSP
- AI Audio
- Machine Learning Audio
- Vocal Processing
- Native Instruments
- Soundwide
---
