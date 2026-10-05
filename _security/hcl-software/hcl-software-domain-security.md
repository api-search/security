---
api_specs:
- filename: hcl-software-stwebapi-api-openapi.yml
  format: yaml
  label: HCLSoftware Stwebapi API
  slug: hcl-software-stwebapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcl-software/refs/heads/main/openapi/hcl-software-stwebapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hcl-software.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.hcl-software.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hcl Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HCLSoftware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HCLSoftware
provider_slug: hcl-software
slug: hcl-software-domain-security
source_filename: hcl-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hcl-software.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hcl-software.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hcl-software/refs/heads/main/security/hcl-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software
- Enterprise
- Artificial Intelligence
- Cloud
---
