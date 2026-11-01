---
api_specs:
- filename: binderwork-com-v1-openapi.json
  format: json
  label: Binderwork API V1 API
  slug: binderwork-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/binderwork-com/openapi/_original/binderwork-com-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: binderwork.com
  spf: true
hosts:
- cert_expires: Dec 31 10:22:36 2026 GMT
  host: binderwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Binderwork Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for binderwork-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: binderwork-com
provider_slug: binderwork-com
slug: binderwork-com-domain-security
source_filename: binderwork-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: binderwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 10:22:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: binderwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/binderwork-com/security/binderwork-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- OpenSource
- DocumentManagement
- ESignature
- StartupTools
---
