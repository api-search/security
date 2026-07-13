---
api_specs:
- filename: matternet-openapi.yml
  format: yaml
  label: Matternet Cloud Software Platform
  slug: matternet-cloud-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matternet/refs/heads/main/openapi/matternet-openapi.yml
- filename: matternet-openapi.yml
  format: yaml
  label: Matternet Logistics Integration
  slug: matternet-logistics-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matternet/refs/heads/main/openapi/matternet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: matternet.com
  spf: true
hosts:
- cert_expires: Sep 27 14:22:23 2026 GMT
  host: www.matternet.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matternet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matternet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matternet
provider_slug: matternet
slug: matternet-domain-security
source_filename: matternet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.matternet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:22:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: matternet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matternet/refs/heads/main/security/matternet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drone Delivery
- Logistics
- Healthcare
- Autonomous
- UAS
- Telemetry
---
