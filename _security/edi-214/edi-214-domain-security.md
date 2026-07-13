---
api_specs:
- filename: stedi-edi214-openapi.yml
  format: yaml
  label: EDI 214 Transportation Carrier Shipment Status Message
  slug: edi-214-standard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edi-214/refs/heads/main/openapi/stedi-edi214-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: x12.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stedi.com
  spf: true
hosts:
- cert_expires: Oct  9 13:47:26 2026 GMT
  host: x12.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 03:39:35 2026 GMT
  host: www.stedi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.stedi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Edi 214 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for edi-214, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: edi-214
provider_slug: edi-214
slug: edi-214-domain-security
source_filename: edi-214-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x12.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:47:26 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.stedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:39:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stedi.com\n  https: false\ndomains:\n- domain: x12.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stedi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edi-214/refs/heads/main/security/edi-214-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
