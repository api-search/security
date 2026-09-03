---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: turionspace.com
  spf: true
hosts:
- cert_expires: Oct 22 21:27:02 2026 GMT
  host: www.turionspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: starfire.turionspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 20:27:28 2026 GMT
  host: api.app.turionspace.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turion Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turion Space, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Turion Space
provider_slug: turion-space
slug: turion-space-domain-security
source_filename: turion-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.turionspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 21:27:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: starfire.turionspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: api.app.turionspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 20:27:28 2026 GMT\n  hsts: null\ndomains:\n- domain: turionspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turion-space/refs/heads/main/security/turion-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Satellites
- Space Domain Awareness
- Non-Earth Imaging
- Earth Observation
- Aerospace
- Defense
- Geospatial
- Imagery
---
