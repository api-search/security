---
api_specs:
- filename: moxiedocs-com-check-drift-api-openapi.yml
  format: yaml
  label: moxiedocs-com Check Drift API
  slug: moxiedocs-com-check-drift-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxiedocs-com/openapi/moxiedocs-com-check-drift-api-openapi.yml
- filename: moxiedocs-com-docs-api-openapi.yml
  format: yaml
  label: moxiedocs-com Docs API
  slug: moxiedocs-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxiedocs-com/openapi/moxiedocs-com-docs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: moxiedocs.com
  spf: true
hosts:
- cert_expires: Dec 19 01:46:26 2026 GMT
  host: moxiedocs.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moxiedocs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for moxiedocs-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: moxiedocs-com
provider_slug: moxiedocs-com
slug: moxiedocs-com-domain-security
source_filename: moxiedocs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moxiedocs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:46:26 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: moxiedocs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/moxiedocs-com/security/moxiedocs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Documentation
- AI
- GitHub
- Automation
- Developer Tools
---
