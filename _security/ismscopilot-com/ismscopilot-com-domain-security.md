---
api_specs:
- filename: ismscopilot-com-docs-api-openapi.yml
  format: yaml
  label: ISMS Copilot Docs API
  slug: ismscopilot-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismscopilot-com/openapi/ismscopilot-com-docs-api-openapi.yml
- filename: ismscopilot-com-public-feeds-api-openapi.yml
  format: yaml
  label: ISMS Copilot Public Feeds API
  slug: ismscopilot-com-public-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismscopilot-com/openapi/ismscopilot-com-public-feeds-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ismscopilot.com
  spf: true
hosts:
- cert_expires: Dec 30 02:25:37 2026 GMT
  host: ismscopilot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ISMS Copilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISMS Copilot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ISMS Copilot
provider_slug: ismscopilot-com
slug: ismscopilot-com-domain-security
source_filename: ismscopilot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ismscopilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 02:25:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ismscopilot.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ismscopilot-com/security/ismscopilot-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GRC
- Artificial Intelligence
- Compliance
- ISO 27001
- SOC 2
---
