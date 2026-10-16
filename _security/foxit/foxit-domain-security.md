---
api_specs:
- filename: foxit-openapi-generated.yml
  format: yaml
  label: Foxit eSign API
  slug: foxit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foxit/refs/heads/main/openapi/_ae-authored/foxit-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foxit.com
  spf: true
hosts:
- cert_expires: Feb  2 12:33:51 2027 GMT
  host: foxit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foxit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foxit eSign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foxit eSign
provider_slug: foxit
slug: foxit-domain-security
source_filename: foxit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foxit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 12:33:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foxit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foxit/refs/heads/main/security/foxit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSignature
- Document Management
- PDF
- Cloud APIs
- Enterprise Software
- Workflow Automation
---
