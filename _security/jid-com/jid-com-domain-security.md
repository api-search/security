---
api_specs:
- filename: jid-com-monitors-api-openapi.yml
  format: yaml
  label: jid-com Monitors API
  slug: jid-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-monitors-api-openapi.yml
- filename: jid-com-qualify-api-openapi.yml
  format: yaml
  label: jid-com Qualify API
  slug: jid-com-qualify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-qualify-api-openapi.yml
- filename: jid-com-screen-api-openapi.yml
  format: yaml
  label: jid-com Screen API
  slug: jid-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-screen-api-openapi.yml
- filename: jid-com-search-api-openapi.yml
  format: yaml
  label: jid-com Search API
  slug: jid-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-search-api-openapi.yml
- filename: jid-com-signal-api-openapi.yml
  format: yaml
  label: jid-com Signal API
  slug: jid-com-signal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-signal-api-openapi.yml
- filename: jid-com-verify-api-openapi.yml
  format: yaml
  label: jid-com Verify API
  slug: jid-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jid.com
  spf: true
hosts:
- cert_expires: Jan  2 22:50:18 2027 GMT
  host: jid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jid Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jid-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: jid-com
provider_slug: jid-com
slug: jid-com-domain-security
source_filename: jid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 22:50:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jid-com/security/jid-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trust
- AI
- Compliance
- Data
- Verification
---
