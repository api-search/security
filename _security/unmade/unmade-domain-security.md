---
api_specs:
- filename: unmade-embed-v2-openapi.json
  format: json
  label: Unmade Integration API (V2)
  slug: unmade-integration-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-embed-v2-openapi.json
- filename: unmade-embed-v1-openapi.json
  format: json
  label: Unmade Integration API (V1)
  slug: unmade-integration-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-embed-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unmade.com
  spf: true
hosts:
- cert_expires: Sep 10 07:26:00 2026 GMT
  host: unmade.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: partner-subdomain.embed.unmade.com
  https: false
kind: domain-security
layout: security
method: probed
name: Unmade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unmade, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unmade
provider_slug: unmade
slug: unmade-domain-security
source_filename: unmade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unmade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:26:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-subdomain.embed.unmade.com\n  https: false\ndomains:\n- domain: unmade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/security/unmade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fashion
- Apparel
- Manufacturing
- Customization
- eCommerce
- On-Demand Production
- Embedded Commerce
---
