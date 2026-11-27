---
api_specs:
- filename: muninx-com-openapi-generated.yml
  format: yaml
  label: Muninx API
  slug: muninx-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muninx-com/openapi/_ae-authored/muninx-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: muninx.com
  spf: true
hosts:
- cert_expires: Jan 27 19:50:10 2027 GMT
  host: muninx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Muninx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Muninx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Muninx
provider_slug: muninx-com
slug: muninx-com-domain-security
source_filename: muninx-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: muninx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:50:10 2027 GMT\n  hsts: false\ndomains:\n- domain: muninx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/muninx-com/security/muninx-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Help Desk
- Software-as-a-Service
- Customer Service
- Artificial Intelligence
- Free Tier
---
