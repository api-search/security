---
api_specs:
- filename: electricity-maps-openapi.yml
  format: yaml
  label: Electricity Maps API
  slug: electricity-maps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-maps/refs/heads/main/openapi/electricity-maps-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: electricitymaps.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: electricitymap.org
  spf: true
hosts:
- cert_expires: Aug 17 04:55:10 2026 GMT
  host: www.electricitymaps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 11:24:25 2026 GMT
  host: app.electricitymaps.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:42:36 2026 GMT
  host: api.electricitymap.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electricity Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electricity Maps, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Electricity Maps
provider_slug: electricity-maps
slug: electricity-maps-domain-security
source_filename: electricity-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.electricitymaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 04:55:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.electricitymaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.electricitymap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:42:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: electricitymaps.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: electricitymap.org\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electricity-maps/refs/heads/main/security/electricity-maps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Electricity
- Carbon Intensity
- Sustainability
- Climate
- Grid Data
---
