---
api_specs:
- filename: aritma-openapi-generated.yml
  format: yaml
  label: Aritma API
  slug: aritma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/_ae-authored/aritma-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aritma.com
  spf: true
hosts:
- cert_expires: Jan  9 18:11:49 2027 GMT
  host: aritma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aritma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aritma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aritma
provider_slug: aritma
slug: aritma-domain-security
source_filename: aritma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aritma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:11:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aritma.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/security/aritma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Automation
- B2B
- Payments
---
