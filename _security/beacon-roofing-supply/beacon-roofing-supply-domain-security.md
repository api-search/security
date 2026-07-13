---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Beacon PRO+ API
  slug: beacon-pro-plus
  spec_type: OpenAPI
  url: https://beaconproplus.com/swagger/all_api/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: becn.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beaconproplus.com
  spf: true
hosts:
- cert_expires: Sep 28 13:34:36 2026 GMT
  host: www.becn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 03:59:59 2026 GMT
  host: www.beaconproplus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 03:59:59 2026 GMT
  host: beaconproplus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beacon Roofing Supply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beacon Roofing Supply, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beacon Roofing Supply
provider_slug: beacon-roofing-supply
slug: beacon-roofing-supply-domain-security
source_filename: beacon-roofing-supply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.becn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:34:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.beaconproplus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 03:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: beaconproplus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 03:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: becn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: beaconproplus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/security/beacon-roofing-supply-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Distribution
- Roofing
- Building Materials
- E-Commerce
- Fortune 1000
---
