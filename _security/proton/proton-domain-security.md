---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Proton API
  slug: proton-api
  spec_type: Postman
  url: https://api.proton.ai/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: proton.ai
  spf: true
hosts:
- cert_expires: Sep 11 00:00:35 2026 GMT
  host: www.proton.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 22:37:42 2026 GMT
  host: api.proton.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proton.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Proton.ai
provider_slug: proton
slug: proton-domain-security
source_filename: proton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proton.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:00:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.proton.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 22:37:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: proton.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proton/refs/heads/main/security/proton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Distribution
- Wholesale
- B2B
- Sales
- Recommendations
- CRM
- e-Commerce
---
