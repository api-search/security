---
api_specs:
- filename: otonomo-fleet-openapi.yml
  format: yaml
  label: Otonomo Fleet API
  slug: otonomo-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otonomo/refs/heads/main/openapi/otonomo-fleet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: otonomo.io
  spf: true
hosts:
- host: otonomo.io
  https: false
- cert_expires: Oct  2 17:45:00 2026 GMT
  host: docs.otonomo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 15:44:35 2026 GMT
  host: api.otonomo.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Otonomo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otonomo, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Otonomo
provider_slug: otonomo
slug: otonomo-domain-security
source_filename: otonomo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otonomo.io\n  https: false\n- host: docs.otonomo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:45:00 2026 GMT\n  hsts: null\n- host: api.otonomo.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  7 15:44:35 2026 GMT\n  hsts: null\ndomains:\n- domain: otonomo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otonomo/refs/heads/main/security/otonomo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Connected Vehicles
- Automotive
- Fleet Management
- Telematics
- Vehicle Data
- Mobility
- IoT
- Location
- Connected Car
---
