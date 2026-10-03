---
api_specs:
- filename: rsa-com-openapi-generated.yml
  format: yaml
  label: RSA API
  slug: rsa-com-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsa-com/refs/heads/main/openapi/_ae-authored/rsa-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rsa.com
  spf: true
hosts:
- cert_expires: Nov 26 06:57:50 2026 GMT
  host: www.rsa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rsa Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RSA
provider_slug: rsa-com
slug: rsa-com-domain-security
source_filename: rsa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rsa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 06:57:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rsa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsa-com/refs/heads/main/security/rsa-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Management
- Multi-Factor Authentication
- Passwordless
- Identity Governance
- Cloud IAM
- Government
- Financial Services
---
