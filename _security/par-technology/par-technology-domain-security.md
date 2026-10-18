---
api_specs:
- filename: par-technology-auth-api-openapi.yml
  format: yaml
  label: PAR Technology Auth API
  slug: par-technology-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-auth-api-openapi.yml
- filename: par-technology-discounts-api-openapi.yml
  format: yaml
  label: PAR Technology Discounts API
  slug: par-technology-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-discounts-api-openapi.yml
- filename: par-technology-pos-api-openapi.yml
  format: yaml
  label: PAR Technology Pos API
  slug: par-technology-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-pos-api-openapi.yml
- filename: par-technology-redemptions-api-openapi.yml
  format: yaml
  label: PAR Technology Redemptions API
  slug: par-technology-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-redemptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: partech.com
  spf: true
hosts:
- cert_expires: Dec 18 21:13:51 2026 GMT
  host: partech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Par Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PAR Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PAR Technology
provider_slug: par-technology
slug: par-technology-domain-security
source_filename: par-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 21:13:51 2026 GMT\n  hsts: false\ndomains:\n- domain: partech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/security/par-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hospitality
- Point-of-Sale
- Loyalty
- Retail
---
