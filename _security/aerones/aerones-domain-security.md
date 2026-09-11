---
api_specs:
- filename: aerones-operations-hub-openapi.json
  format: json
  label: Aerones Operations Hub API
  slug: aerones-operations-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerones/refs/heads/main/openapi/aerones-operations-hub-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aerones.com
  spf: true
hosts:
- cert_expires: Oct 29 08:36:42 2026 GMT
  host: aerones.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 22:26:25 2026 GMT
  host: operations.aerones.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aerones Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerones, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aerones
provider_slug: aerones
slug: aerones-domain-security
source_filename: aerones-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aerones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 08:36:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: operations.aerones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 22:26:25 2026 GMT\n  hsts: false\ndomains:\n- domain: aerones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerones/refs/heads/main/security/aerones-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wind Energy
- Renewable Energy
- Robotics
- Drones
- Inspection
- Field Service Management
- Asset Management
- Industrial
- Energy
- Maintenance
- Latvia
---
