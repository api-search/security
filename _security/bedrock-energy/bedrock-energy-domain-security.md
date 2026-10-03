---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bedrockenergy.com
  spf: true
hosts:
- cert_expires: Dec 24 13:55:43 2026 GMT
  host: bedrockenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bedrock Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bedrock Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bedrock Energy
provider_slug: bedrock-energy
slug: bedrock-energy-domain-security
source_filename: bedrock-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bedrockenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 13:55:43 2026 GMT\n  hsts: false\ndomains:\n- domain: bedrockenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bedrock-energy/refs/heads/main/security/bedrock-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geothermal
- Energy
- HVAC
- Cleantech
---
