---
api_specs:
- filename: catalystedgescanner-com-openapi-generated.yml
  format: yaml
  label: Catalyst Edge API
  slug: catalystedgescanner-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalystedgescanner-com/openapi/_ae-authored/catalystedgescanner-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: catalystedgescanner.com
  spf: true
hosts:
- cert_expires: Dec 21 05:35:27 2026 GMT
  host: catalystedgescanner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Catalyst Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catalyst Edge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Catalyst Edge
provider_slug: catalystedgescanner-com
slug: catalystedgescanner-com-domain-security
source_filename: catalystedgescanner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalystedgescanner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 05:35:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: catalystedgescanner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/catalystedgescanner-com/security/catalystedgescanner-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- SEC
- Market Data
- Analytics
- Platform
---
