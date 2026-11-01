---
api_specs:
- filename: placid-openai-api-openapi.yml
  format: yaml
  label: Placid Openai API
  slug: placid-openai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placid/openapi/placid-openai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: placid.app
  spf: true
hosts:
- cert_expires: Dec 26 03:28:07 2026 GMT
  host: placid.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Placid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Placid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Placid
provider_slug: placid
slug: placid-domain-security
source_filename: placid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: placid.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 03:28:07 2026 GMT\n  hsts: false\ndomains:\n- domain: placid.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/placid/security/placid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automation
- Creative
- API
- Image-Generation
- No-Code
---
