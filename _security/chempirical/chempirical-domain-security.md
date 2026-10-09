---
api_specs:
- filename: chempirical-openapi-generated.yml
  format: yaml
  label: Chempirical (Nitramine) API
  slug: chempirical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chempirical/refs/heads/main/openapi/_ae-authored/chempirical-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chempirical.com
  spf: true
hosts:
- cert_expires: Nov 20 06:33:23 2026 GMT
  host: chempirical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chempirical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chempirical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chempirical
provider_slug: chempirical
slug: chempirical-domain-security
source_filename: chempirical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chempirical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 06:33:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chempirical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chempirical/refs/heads/main/security/chempirical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chemistry
- Compounds
- Reactions
- Science
- Open Data
- JSON API
---
