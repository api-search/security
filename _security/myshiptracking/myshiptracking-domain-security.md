---
api_specs:
- filename: myshiptracking-account-api-openapi.yml
  format: yaml
  label: MyShipTracking Account API
  slug: myshiptracking-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-account-api-openapi.yml
- filename: myshiptracking-ports-api-openapi.yml
  format: yaml
  label: MyShipTracking Ports API
  slug: myshiptracking-ports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-ports-api-openapi.yml
- filename: myshiptracking-vessels-api-openapi.yml
  format: yaml
  label: MyShipTracking Vessels API
  slug: myshiptracking-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-vessels-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myshiptracking.com
  spf: true
  spf_record: v=spf1 mx a ip4:178.162.215.171 ip4:178.162.215.136 include:spf.mandrillapp.com include:_spf.google.com ~all
hosts:
- cert_expires: Sep 12 01:42:39 2026 GMT
  cert_not_before: Jun 14 01:42:40 2026 GMT
  host: www.myshiptracking.com
  hsts: false
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:42:39 2026 GMT
  cert_not_before: Jun 14 01:42:40 2026 GMT
  host: myshiptracking.com
  hsts: false
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:42:39 2026 GMT
  cert_not_before: Jun 14 01:42:40 2026 GMT
  host: api.myshiptracking.com
  hsts: false
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myshiptracking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyShipTracking, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyShipTracking
provider_slug: myshiptracking
slug: myshiptracking-domain-security
source_filename: myshiptracking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myshiptracking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: Jun 14 01:42:40 2026 GMT\n  cert_expires: Sep 12 01:42:39 2026 GMT\n  server: cloudflare\n  hsts: false\n- host: myshiptracking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: Jun 14 01:42:40 2026 GMT\n  cert_expires: Sep 12 01:42:39 2026 GMT\n  server: cloudflare\n  hsts: false\n- host: api.myshiptracking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: Jun 14 01:42:40 2026 GMT\n  cert_expires: Sep 12 01:42:39 2026 GMT\n  server: cloudflare\n  hsts: false\ndomains:\n- domain: myshiptracking.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 mx a ip4:178.162.215.171 ip4:178.162.215.136 include:spf.mandrillapp.com include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: none\nnotes: >-\n  All three hosts terminate TLS 1.3 behind\
  \ Cloudflare with a shared certificate\n  (valid Jun 14 - Sep 12 2026). No HSTS response header was observed on the\n  document root of any host at probe time. SPF is published (soft-fail ~all,\n  Mandrill + Google senders). DMARC is published but set to p=none (monitor\n  only). No DNSSEC and no CAA records were found for myshiptracking.com.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/security/myshiptracking-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vessel Tracking
- AIS
- Maritime
- Ship Tracking
- Real-Time Data
- Ships
- Port Calls
- Maritime Data
- Location
- Fleet Tracking
---
