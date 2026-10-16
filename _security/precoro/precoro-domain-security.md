---
api_specs:
- filename: precoro-openapi-generated.yml
  format: yaml
  label: Precoro API
  slug: precoro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/_ae-authored/precoro-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: precoro.com
  spf: true
hosts:
- cert_expires: Dec 25 23:47:20 2026 GMT
  host: www.precoro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Precoro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Precoro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Precoro
provider_slug: precoro
slug: precoro-domain-security
source_filename: precoro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.precoro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:47:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: precoro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/security/precoro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Procurement
- Spend Management
- Vendor Management
- Purchase-to-Pay
- AP Automation
- Contract Management
- AI Procurement
---
