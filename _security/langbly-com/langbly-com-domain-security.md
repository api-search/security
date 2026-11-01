---
api_specs:
- filename: langbly-com-translation-api-openapi.yml
  format: yaml
  label: langbly-com Translation API
  slug: langbly-com-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbly-com/openapi/langbly-com-translation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: langbly.com
  spf: true
hosts:
- cert_expires: Dec 22 11:57:31 2026 GMT
  host: langbly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Langbly Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for langbly-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: langbly-com
provider_slug: langbly-com
slug: langbly-com-domain-security
source_filename: langbly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: langbly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 11:57:31 2026 GMT\n  hsts: false\ndomains:\n- domain: langbly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/langbly-com/security/langbly-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Translation
- API
- Localization
- SaaS
- Machine-Learning
---
