---
api_specs:
- filename: opensky-rest-api.json
  format: json
  label: OpenSky Network REST API
  slug: opensky-network-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensky/refs/heads/main/openapi/opensky-rest-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opensky-network.org
  spf: true
hosts:
- cert_expires: Sep  4 10:59:22 2026 GMT
  host: opensky-network.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 18:06:34 2026 GMT
  host: trino.opensky-network.org
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSky Network, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenSky Network
provider_slug: opensky
slug: opensky-domain-security
source_filename: opensky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensky-network.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:59:22 2026 GMT\n  hsts: null\n- host: trino.opensky-network.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 18:06:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: opensky-network.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensky/refs/heads/main/security/opensky-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- Flight Tracking
- ADS-B
- Aircraft
- Airport
- Real-Time
- Historical Data
---
