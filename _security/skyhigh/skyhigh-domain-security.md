---
api_specs:
- filename: skyhigh-incidents-openapi-original.yml
  format: yaml
  label: Skyhigh Security SSE Incidents API
  slug: skyhigh-security-sse-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/openapi/skyhigh-incidents-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skyhighsecurity.com
  spf: true
hosts:
- cert_expires: Aug 26 06:37:02 2026 GMT
  host: www.skyhighsecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skyhigh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skyhigh Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skyhigh Security
provider_slug: skyhigh
slug: skyhigh-domain-security
source_filename: skyhigh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skyhighsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:37:02 2026 GMT\n  hsts: false\ndomains:\n- domain: skyhighsecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/security/skyhigh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- Security Service Edge
- CASB
- Secure Web Gateway
- Data Loss Prevention
- Cloud Security
- Zero Trust
- SASE
---
