---
api_specs:
- filename: usehaystack-openapi-generated.yml
  format: yaml
  label: Haystack Analytics API
  slug: usehaystack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usehaystack/openapi/_ae-authored/usehaystack-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usehaystack.io
  spf: true
hosts:
- cert_expires: Dec 10 06:39:44 2026 GMT
  host: usehaystack.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 15:58:11 2026 GMT
  host: help.usehaystack.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Usehaystack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haystack Analytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Haystack Analytics
provider_slug: usehaystack
slug: usehaystack-domain-security
source_filename: usehaystack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usehaystack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:39:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.usehaystack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 15:58:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usehaystack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/usehaystack/security/usehaystack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DeliveryOps
- Product Management
- Engineering
- Analytics
---
