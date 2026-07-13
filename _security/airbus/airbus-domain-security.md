---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airbus.com
  spf: true
hosts:
- cert_expires: Oct  1 10:03:55 2026 GMT
  host: www.airbus.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 12:49:46 2026 GMT
  host: api.oneatlas.airbus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 10:40:28 2026 GMT
  host: authenticate.foundation.api.oneatlas.airbus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airbus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airbus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airbus
provider_slug: airbus
slug: airbus-domain-security
source_filename: airbus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: api.oneatlas.airbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:49:46 2026 GMT\n  hsts: false\n- host: authenticate.foundation.api.oneatlas.airbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 10:40:28 2026 GMT\n  hsts: null\ndomains:\n- domain: airbus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbus/refs/heads/main/security/airbus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Defense
- Manufacturing
- Aviation
- Earth Observation
- Satellite Imagery
---
