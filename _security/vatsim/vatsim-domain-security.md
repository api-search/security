---
api_specs:
- filename: openapi.json
  format: json
  label: VATSIM Core API
  slug: vatsim-core-api
  spec_type: OpenAPI
  url: https://api.vatsim.net/v2/openapi.json
- filename: openapi.json
  format: json
  label: VATSIM Data API
  slug: vatsim-data-api
  spec_type: OpenAPI
  url: https://data.vatsim.net/openapi.json
- filename: metar.yaml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/metar.yaml
- filename: connect.yaml
  format: yaml
  label: VATSIM Connect API
  slug: vatsim-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/connect.yaml
- filename: slurper.yaml
  format: yaml
  label: VATSIM Slurper API
  slug: vatsim-slurper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/slurper.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: vatsim.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vatsim.net
  spf: true
hosts:
- cert_expires: Sep 15 13:09:37 2026 GMT
  host: vatsim.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:02:46 2026 GMT
  host: api.vatsim.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:02:46 2026 GMT
  host: data.vatsim.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vatsim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VATSIM, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: VATSIM
provider_slug: vatsim
slug: vatsim-domain-security
source_filename: vatsim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vatsim.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:09:37 2026 GMT\n  hsts: false\n- host: api.vatsim.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:02:46 2026 GMT\n  hsts: false\n- host: data.vatsim.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:02:46 2026 GMT\n  hsts: false\ndomains:\n- domain: vatsim.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: vatsim.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/security/vatsim-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Aviation
- Flight Simulation
- Air Traffic Control
- Real-Time Data
- Community
---
