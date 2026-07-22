---
api_specs:
- filename: zego-partner-openapi.yml
  format: yaml
  label: Zego Partner API
  slug: zego-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zego/refs/heads/main/openapi/zego-partner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zego.com
  spf: true
hosts:
- cert_expires: Sep 15 17:30:27 2026 GMT
  host: www.zego.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: developer.zego.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 17:30:27 2026 GMT
  host: api.zego.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zego Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zego, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zego
provider_slug: zego
slug: zego-domain-security
source_filename: zego-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zego.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.zego.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.zego.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: zego.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zego/refs/heads/main/security/zego-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Motor Insurance
- Gig Economy
- Telematics
- Fleet Insurance
- Public Liability
- Partner API
---
