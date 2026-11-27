---
api_specs:
- filename: invisibleexit-com-agent-api-openapi.yml
  format: yaml
  label: Invisible Exit Agent API
  slug: invisibleexit-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invisibleexit-com/openapi/invisibleexit-com-agent-api-openapi.yml
- filename: invisibleexit-com-embed-api-openapi.yml
  format: yaml
  label: Invisible Exit Embed API
  slug: invisibleexit-com-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invisibleexit-com/openapi/invisibleexit-com-embed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: invisibleexit.com
  spf: true
hosts:
- cert_expires: Dec 23 13:00:03 2026 GMT
  host: invisibleexit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Invisible Exit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invisible Exit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Invisible Exit
provider_slug: invisibleexit-com
slug: invisibleexit-com-domain-security
source_filename: invisibleexit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invisibleexit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 13:00:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: invisibleexit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/invisibleexit-com/security/invisibleexit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Software-as-a-Service
- Entrepreneurship
- Privacy
---
