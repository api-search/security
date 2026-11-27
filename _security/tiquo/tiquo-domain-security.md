---
api_specs:
- filename: tiquo-openapi-generated.yml
  format: yaml
  label: Tiquo Hospitality API
  slug: tiquo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tiquo/openapi/_ae-authored/tiquo-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tiquo.co
  spf: true
hosts:
- cert_expires: Jan 11 11:13:25 2027 GMT
  host: www.tiquo.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tiquo Hospitality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tiquo Hospitality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tiquo Hospitality
provider_slug: tiquo
slug: tiquo-domain-security
source_filename: tiquo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiquo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 11:13:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tiquo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tiquo/security/tiquo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Point-of-Sale
- Booking
- Payments
- Membership
- Marketing
- Hospitality Software
- Multi‑location Management
- Analytics
---
