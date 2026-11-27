---
api_specs:
- filename: liqwall-com-openapi-generated.yml
  format: yaml
  label: Liqwall API
  slug: liqwall-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liqwall-com/openapi/_ae-authored/liqwall-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liqwall.com
  spf: true
hosts:
- cert_expires: Jan  9 18:03:52 2027 GMT
  host: liqwall.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Liqwall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liqwall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liqwall
provider_slug: liqwall-com
slug: liqwall-com-domain-security
source_filename: liqwall-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liqwall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:03:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liqwall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/liqwall-com/security/liqwall-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Data
- Visualization
- Market Data
- Real-Time
- Company
---
