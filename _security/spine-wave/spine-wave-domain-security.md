---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spinewave.com
  spf: true
hosts:
- cert_expires: Jan  2 03:28:50 2027 GMT
  host: spinewave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spine Wave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spine Wave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spine Wave
provider_slug: spine-wave
slug: spine-wave-domain-security
source_filename: spine-wave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spinewave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 03:28:50 2027 GMT\n  hsts: false\ndomains:\n- domain: spinewave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/spine-wave/security/spine-wave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Devices
- Spine Surgery
- Innovation
- Healthcare
- Biotechnology
- Company
---
