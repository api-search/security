---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bedrockocean.com
  spf: true
hosts:
- cert_expires: Oct  5 14:38:45 2026 GMT
  host: www.bedrockocean.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bedrock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bedrock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bedrock
provider_slug: bedrock
slug: bedrock-domain-security
source_filename: bedrock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bedrockocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:38:45 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: bedrockocean.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bedrock/refs/heads/main/security/bedrock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Ocean Data
- Seafloor Mapping
- Marine
- Autonomous Vehicles
- Geospatial
- Offshore Energy
- Data Platform
---
