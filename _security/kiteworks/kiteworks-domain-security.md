---
api_specs:
- filename: kiteworks-core-openapi-original.json
  format: json
  label: Kiteworks Core API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/openapi/kiteworks-core-openapi-original.json
- filename: kiteworks-pubsub-openapi-original.yml
  format: yaml
  label: Kiteworks PubSub Consumer API
  slug: pubsub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/openapi/kiteworks-pubsub-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kiteworks.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.kiteworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: developer.kiteworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kiteworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiteworks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kiteworks
provider_slug: kiteworks
slug: kiteworks-domain-security
source_filename: kiteworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kiteworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kiteworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kiteworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnote: baseURL hosts are per-tenant (Kiteworks is a self-hosted/private-cloud appliance);\n  the template placeholder host your.kiteworks.domain was excluded from probing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/security/kiteworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Secure File Sharing
- Managed File Transfer
- Secure Email
- Data Governance
- Regulatory Compliance
- Content Security
- Private Data Network
- CMMC
- SCIM
---
