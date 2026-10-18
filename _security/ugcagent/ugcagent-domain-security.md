---
api_specs:
- filename: ugcagent-messages-api-openapi.yml
  format: yaml
  label: UGC Agent Messages API
  slug: ugcagent-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ugcagent/refs/heads/main/openapi/ugcagent-messages-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ugcagent.app
  spf: true
hosts:
- cert_expires: Nov 25 19:43:49 2026 GMT
  host: ugcagent.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ugcagent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UGC Agent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: UGC Agent
provider_slug: ugcagent
slug: ugcagent-domain-security
source_filename: ugcagent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ugcagent.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 19:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ugcagent.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ugcagent/refs/heads/main/security/ugcagent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- UGC
- Marketing
- Data
- Creators
---
