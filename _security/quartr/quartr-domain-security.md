---
api_specs:
- filename: quartr-openapi-generated.yml
  format: yaml
  label: Quartr API
  slug: quartr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartr/refs/heads/main/openapi/_ae-authored/quartr-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quartr.com
  spf: true
hosts:
- cert_expires: Nov 24 17:43:58 2026 GMT
  host: quartr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quartr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quartr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quartr
provider_slug: quartr
slug: quartr-domain-security
source_filename: quartr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quartr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 17:43:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quartr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quartr/refs/heads/main/security/quartr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Finance
- Data
- Research
---
