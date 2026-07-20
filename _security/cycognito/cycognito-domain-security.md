---
api_specs:
- filename: cycognito-v1-openapi-original.json
  format: json
  label: CyCognito API V1
  slug: cycognito-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-v1-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cycognito.com
  spf: true
hosts:
- cert_expires: Oct 11 11:31:18 2026 GMT
  host: www.cycognito.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cycognito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyCognito, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CyCognito
provider_slug: cycognito
slug: cycognito-domain-security
source_filename: cycognito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cycognito.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 11:31:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cycognito.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/security/cycognito-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Attack Surface Management
- Exposure Management
- Security
- Vulnerability Management
- Cloud Security
- API Security
---
