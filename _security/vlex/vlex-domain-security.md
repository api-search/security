---
api_specs:
- filename: vlex-iceberg-anonymization-openapi.yml
  format: yaml
  label: vLex Iceberg Anonymization API
  slug: iceberg-anonymization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/openapi/vlex-iceberg-anonymization-openapi.yml
- filename: vlex-iceberg-legal-research-openapi.yml
  format: yaml
  label: vLex Iceberg Legal Research API
  slug: iceberg-legal-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/openapi/vlex-iceberg-legal-research-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vlex.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: vlex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 06:07:07 2026 GMT
  host: developer.vlex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.vlex.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vlex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vLex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: vLex
provider_slug: vlex
slug: vlex-domain-security
source_filename: vlex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vlex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.vlex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:07:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vlex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: vlex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/security/vlex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Classification
- Legal Research
- Legal Tech
- Natural Language Processing
- Privacy
---
