---
api_specs:
- filename: johnson-and-johnson-lifescan-api-openapi.yml
  format: yaml
  label: Johnson & Johnson LifeScan API
  slug: lifescan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-and-johnson/refs/heads/main/openapi/johnson-and-johnson-lifescan-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jnj.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lifescan.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.jnj.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.lifescan.com
  https: false
kind: domain-security
layout: security
method: probed
name: Johnson And Johnson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Johnson & Johnson, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Johnson & Johnson
provider_slug: johnson-and-johnson
slug: johnson-and-johnson-domain-security
source_filename: johnson-and-johnson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jnj.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: api.lifescan.com\n  https: false\ndomains:\n- domain: jnj.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lifescan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnson-and-johnson/refs/heads/main/security/johnson-and-johnson-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Medical Devices
- Diabetes
- Blood Glucose
- Pharmaceuticals
- Fortune 100
---
