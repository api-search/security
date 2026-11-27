---
api_specs:
- filename: lettrove-com-server-api-api-openapi.yml
  format: yaml
  label: Lettrove Server API
  slug: lettrove-com-server-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lettrove-com/openapi/lettrove-com-server-api-api-openapi.yml
- filename: lettrove-com-webhooks-api-openapi.yml
  format: yaml
  label: Lettrove Webhooks API
  slug: lettrove-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lettrove-com/openapi/lettrove-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lettrove.com
  spf: true
hosts:
- cert_expires: Jan  7 04:09:48 2027 GMT
  host: lettrove.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lettrove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lettrove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lettrove
provider_slug: lettrove-com
slug: lettrove-com-domain-security
source_filename: lettrove-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lettrove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 04:09:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lettrove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lettrove-com/security/lettrove-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Email
- Marketing
- Collaboration
---
