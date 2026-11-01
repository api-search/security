---
api_specs:
- filename: usefomo-applications-api-openapi.yml
  format: yaml
  label: FOMO Applications API
  slug: usefomo-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usefomo/openapi/usefomo-applications-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usefomo.com
  spf: true
hosts:
- cert_expires: Dec 22 01:09:24 2026 GMT
  host: usefomo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usefomo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FOMO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FOMO
provider_slug: usefomo
slug: usefomo-domain-security
source_filename: usefomo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usefomo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 01:09:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usefomo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/usefomo/security/usefomo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SocialProof
- Marketing
- SaaS
- ECommerce
---
