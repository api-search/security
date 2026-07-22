---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: urbansky.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: atmosys.com
  spf: false
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: urbansky.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: docs.urbansky.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 20:41:52 2026 GMT
  host: api.ops.atmosys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urban Sky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Sky, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Urban Sky
provider_slug: urban-sky
slug: urban-sky-domain-security
source_filename: urban-sky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbansky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: docs.urbansky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n- host: api.ops.atmosys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:41:52 2026 GMT\n  hsts: null\ndomains:\n- domain: urbansky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atmosys.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-sky/refs/heads/main/security/urban-sky-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Stratospheric Balloons
- Remote Sensing
- Earth Observation
- Aerial Imagery
- Telemetry
- Defense
- Weather
---
