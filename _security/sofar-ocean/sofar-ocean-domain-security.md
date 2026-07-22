---
api_specs:
- filename: sofar-ocean-spotter-openapi.yml
  format: yaml
  label: Spotter & Smart Mooring API
  slug: spotter-smart-mooring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofar-ocean/refs/heads/main/openapi/sofar-ocean-spotter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sofarocean.com
  spf: true
hosts:
- cert_expires: Sep 11 02:56:00 2026 GMT
  host: www.sofarocean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 09:32:42 2026 GMT
  host: docs.sofarocean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.sofarocean.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sofar Ocean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sofar Ocean, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sofar Ocean
provider_slug: sofar-ocean
slug: sofar-ocean-domain-security
source_filename: sofar-ocean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sofarocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:56:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sofarocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:32:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sofarocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sofarocean.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofar-ocean/refs/heads/main/security/sofar-ocean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate
- Ocean Data
- Weather
- Maritime
- Sensors
- IoT
- Environmental Data
- Wave Data
- Buoys
---
