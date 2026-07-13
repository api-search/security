---
api_specs:
- filename: replicate-openapi.yml
  format: yaml
  label: Replicate
  slug: replicate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: replicate.com
  spf: true
hosts:
- cert_expires: Sep 14 21:44:59 2026 GMT
  host: replicate.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 10:33:07 2026 GMT
  host: api.replicate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Replicate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replicate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Replicate
provider_slug: replicate
slug: replicate-domain-security
source_filename: replicate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: replicate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.replicate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 10:33:07 2026 GMT\n  hsts: null\ndomains:\n- domain: replicate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/security/replicate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Machine Learning
- Image Generation
- Language Models
- Model Deployment
---
