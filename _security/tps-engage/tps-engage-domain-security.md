---
api_specs:
- filename: tps-engage-blindspot-pull-api-openapi.yaml
  format: yaml
  label: Blindspot Pull API
  slug: blindspot-pull-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/openapi/tps-engage-blindspot-pull-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: seeblindspot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tpsengage.com
  spf: true
hosts:
- cert_expires: Sep 30 06:12:47 2026 GMT
  host: seeblindspot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: rtb.network.tpsengage.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tps Engage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPS Engage, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TPS Engage
provider_slug: tps-engage
slug: tps-engage-domain-security
source_filename: tps-engage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seeblindspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rtb.network.tpsengage.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: seeblindspot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tpsengage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/security/tps-engage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- DOOH
- Digital Billboards
- Programmatic Advertising
- Media Buying
- Out-of-Home
---
