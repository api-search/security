---
api_specs:
- filename: droplinked-com-openapi-generated.yml
  format: yaml
  label: Droplinked API
  slug: droplinked-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/droplinked-com/openapi/_ae-authored/droplinked-com-openapi-generated.yml
- filename: droplinked-com-openapi-openapi.json
  format: json
  label: Droplinked Openapi API
  slug: droplinked-openapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/droplinked-com/openapi/_original/droplinked-com-openapi-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: droplinked.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: droplinked.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Droplinked Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Droplinked, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Droplinked
provider_slug: droplinked-com
slug: droplinked-com-domain-security
source_filename: droplinked-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: droplinked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: droplinked.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/droplinked-com/security/droplinked-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Artificial Intelligence
- catalog-import
- Online Store
- MCP
---
