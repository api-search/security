---
api_specs:
- filename: llms.txt
  format: yaml
  label: TripleLift Exchange (TLX) API
  slug: triplelift-exchange-tlx-api
  spec_type: OpenAPI
  url: https://triplelift-docs.readme.io/llms.txt
- filename: llms.txt
  format: yaml
  label: TripleLift Supply Publisher API
  slug: triplelift-supply-publisher-api
  spec_type: OpenAPI
  url: https://supply-docs.triplelift.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: triplelift.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: 3lift.com
  spf: false
hosts:
- cert_expires: Sep 20 11:31:07 2026 GMT
  host: triplelift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:50:11 2026 GMT
  host: docs.triplelift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: tlx.3lift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Triplelift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TripleLift, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TripleLift
provider_slug: triplelift
slug: triplelift-domain-security
source_filename: triplelift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triplelift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:31:07 2026 GMT\n  hsts: false\n- host: docs.triplelift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:50:11 2026 GMT\n  hsts: null\n- host: tlx.3lift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: triplelift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 3lift.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triplelift/refs/heads/main/security/triplelift-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Programmatic Advertising
- Native Advertising
- Ad Exchange
- OpenRTB
- Header Bidding
- Connected TV
- Supply Side Platform
- Demand Side Platform
---
