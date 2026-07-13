---
api_specs:
- filename: g-portal-web-api.json
  format: json
  label: G-Portal Web API
  slug: g-portal-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaxa/refs/heads/main/openapi/g-portal-web-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jaxa.jp
  spf: true
hosts:
- cert_expires: Sep 21 05:04:18 2026 GMT
  host: earth.jaxa.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 01:58:30 2026 GMT
  host: data.earth.jaxa.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:04:18 2026 GMT
  host: gportal.jaxa.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jaxa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JAXA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JAXA
provider_slug: jaxa
slug: jaxa-domain-security
source_filename: jaxa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earth.jaxa.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:04:18 2026 GMT\n  hsts: false\n- host: data.earth.jaxa.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 01:58:30 2026 GMT\n  hsts: false\n- host: gportal.jaxa.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:04:18 2026 GMT\n  hsts: false\ndomains:\n- domain: jaxa.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaxa/refs/heads/main/security/jaxa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Space
- Satellite
- Earth Observation
- Remote Sensing
- Geospatial
- Climate
- Environment
- Precipitation
- Greenhouse Gas
- Japan
---
