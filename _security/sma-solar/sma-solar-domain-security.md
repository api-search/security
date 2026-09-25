---
api_specs:
- filename: sma-solar-openapi-generated.yml
  format: yaml
  label: SMA Solar Technology API
  slug: sma-solar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sma-solar/refs/heads/main/openapi/_ae-authored/sma-solar-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sma.de
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.sma.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sma Solar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMA Solar Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SMA Solar Technology
provider_slug: sma-solar
slug: sma-solar-domain-security
source_filename: sma-solar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sma.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sma.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sma-solar/refs/heads/main/security/sma-solar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Solar
- Energy
- Inverters
- Renewables
---
