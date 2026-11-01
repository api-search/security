---
api_specs:
- filename: attlaz-openapi-generated.yml
  format: yaml
  label: Attlaz API
  slug: attlaz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attlaz/openapi/_ae-authored/attlaz-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: attlaz.com
  spf: true
hosts:
- cert_expires: Dec  9 02:37:13 2026 GMT
  host: attlaz.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Attlaz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attlaz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Attlaz
provider_slug: attlaz
slug: attlaz-domain-security
source_filename: attlaz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attlaz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 02:37:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: attlaz.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/attlaz/security/attlaz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Integration
- Automation
- Data Visualization
- Workflows
---
