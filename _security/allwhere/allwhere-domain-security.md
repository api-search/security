---
api_specs:
- filename: allwhere-beta-api-openapi.yml
  format: yaml
  label: allwhere Beta API
  slug: allwhere-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allwhere/refs/heads/main/openapi/allwhere-beta-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allwhere.co
  spf: true
hosts:
- cert_expires: Nov  8 09:09:54 2026 GMT
  host: www.allwhere.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allwhere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for allwhere, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: allwhere
provider_slug: allwhere
slug: allwhere-domain-security
source_filename: allwhere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allwhere.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 09:09:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allwhere.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allwhere/refs/heads/main/security/allwhere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IT
- Asset-Management
- Procurement
- Remote-Workforce
- Enterprise
---
