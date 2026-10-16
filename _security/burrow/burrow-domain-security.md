---
api_specs:
- filename: burrow-openapi-generated.yml
  format: yaml
  label: Burrow API
  slug: burrow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burrow/refs/heads/main/openapi/_ae-authored/burrow-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: useburrow.com
  spf: true
hosts:
- cert_expires: Nov 11 14:51:31 2026 GMT
  host: useburrow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Burrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Burrow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Burrow
provider_slug: burrow
slug: burrow-domain-security
source_filename: burrow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useburrow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:51:31 2026 GMT\n  hsts: false\ndomains:\n- domain: useburrow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burrow/refs/heads/main/security/burrow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SaaS
- Reporting
- Automation
- API
---
