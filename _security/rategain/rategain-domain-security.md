---
api_specs:
- filename: rategain-openapi-generated.yml
  format: yaml
  label: RateGain API
  slug: rategain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rategain/refs/heads/main/openapi/_ae-authored/rategain-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rategain.com
  spf: true
hosts:
- cert_expires: Dec 19 07:10:38 2026 GMT
  host: rategain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rategain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RateGain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RateGain
provider_slug: rategain
slug: rategain-domain-security
source_filename: rategain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rategain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 07:10:38 2026 GMT\n  hsts: false\ndomains:\n- domain: rategain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rategain/refs/heads/main/security/rategain-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hospitality
- TravelTech
- SaaS
- RevenueManagement
---
