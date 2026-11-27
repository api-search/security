---
api_specs:
- filename: lucyesl-com-openapi-generated.yml
  format: yaml
  label: LucyESL API
  slug: lucyesl-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucyesl-com/openapi/_ae-authored/lucyesl-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucyesl.com
  spf: true
hosts:
- cert_expires: Jan  6 19:46:06 2027 GMT
  host: lucyesl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LucyESL Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LucyESL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LucyESL
provider_slug: lucyesl-com
slug: lucyesl-com-domain-security
source_filename: lucyesl-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucyesl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 19:46:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lucyesl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lucyesl-com/security/lucyesl-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Platform
- South Korea
- Privacy
---
