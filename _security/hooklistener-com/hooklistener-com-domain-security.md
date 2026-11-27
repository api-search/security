---
api_specs:
- filename: hooklistener-com-openapi-generated.yml
  format: yaml
  label: Hooklistener API
  slug: hooklistener-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hooklistener-com/openapi/_ae-authored/hooklistener-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hooklistener.com
  spf: true
hosts:
- cert_expires: Jan  7 23:47:48 2027 GMT
  host: hooklistener.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hooklistener Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hooklistener, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hooklistener
provider_slug: hooklistener-com
slug: hooklistener-com-domain-security
source_filename: hooklistener-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hooklistener.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:47:48 2027 GMT\n  hsts: false\ndomains:\n- domain: hooklistener.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hooklistener-com/security/hooklistener-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Webhook
- Artificial Intelligence
- Debugging
- Developer Tool
- MCP
---
