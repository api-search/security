---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jemena.com.au
  spf: true
hosts:
- cert_expires: Sep  5 07:12:37 2026 GMT
  host: www.jemena.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: myservices.jemena.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: sep2.aws.jemena.com.au
  https: false
  note: No listener on port 443. The JEN CSIP-AUS Utility Server listens on port 8443 (production) and the staging host sep2-e2e.aws.jemena.com.au on port 8444 — see the manual entries below.
- host: sep2.aws.jemena.com.au:8443
  hsts: null
  https: true
  mutual_tls: true
  note: TLS handshake succeeds against a private-PKI chain (self-signed certificate in chain, expected for the IEEE 2030.5 SERCA/MICA hierarchy, so public-CA verification fails by design). With verification disabled, GET /sep2/dcap returns HTTP 500 from nginx because no client certificate was presented. Resolves to gsmd-int-prod-01-nlb-680afe73530cbb36.elb.ap-southeast-2.amazonaws.com (AWS NLB, ap-southeast-2).
  probed_manually: true
  public_ca: false
  ssl_verify_result: 19
- host: sep2-e2e.aws.jemena.com.au:8444
  https: null
  mutual_tls: true
  note: Staging. Connection times out from outside Australia, consistent with the documented client-IP allow-listing. Resolves to gsmd-int-nonprod-01-nlb-c1e23f301554325d.elb.ap-southeast-2.amazonaws.com.
  probed_manually: true
- host: myportal.jemena.com.au
  note: Customer/trade login wall; / returns 200, /api and /.well-known/openid-configuration return 403.
  probed_manually: true
- host: poweroutages.jemena.com.au
  note: CloudFront distribution, geo-restricted — returns HTTP 403 outside Australia.
  probed_manually: true
- host: api.jemena.com.au
  note: Resolves via Akamai (api.jemena.com.au.edgekey.net); returns HTTP 503 on /, /openapi.json, /swagger.json and /health. Internal edge, not a public API.
  probed_manually: true
kind: domain-security
layout: security
method: probed
name: Jemena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jemena, probed live across 8 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jemena
provider_slug: jemena
slug: jemena-domain-security
source_filename: jemena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jemena.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: myservices.jemena.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\n- host: sep2.aws.jemena.com.au\n  https: false\n  note: >-\n    No listener on port 443. The JEN CSIP-AUS Utility Server listens on port 8443 (production) and\n    the staging host sep2-e2e.aws.jemena.com.au on port 8444 — see the manual entries below.\n- host: sep2.aws.jemena.com.au:8443\n  https: true\n  mutual_tls: true\n  public_ca: false\n  ssl_verify_result: 19\n  hsts: null\n  probed_manually: true\n  note: >-\n    TLS handshake succeeds against a private-PKI chain (self-signed certificate in chain, expected for\n    the IEEE 2030.5 SERCA/MICA hierarchy, so public-CA verification fails\
  \ by design). With verification\n    disabled, GET /sep2/dcap returns HTTP 500 from nginx because no client certificate was presented.\n    Resolves to gsmd-int-prod-01-nlb-680afe73530cbb36.elb.ap-southeast-2.amazonaws.com (AWS NLB,\n    ap-southeast-2).\n- host: sep2-e2e.aws.jemena.com.au:8444\n  https: null\n  mutual_tls: true\n  probed_manually: true\n  note: >-\n    Staging. Connection times out from outside Australia, consistent with the documented client-IP\n    allow-listing. Resolves to gsmd-int-nonprod-01-nlb-c1e23f301554325d.elb.ap-southeast-2.amazonaws.com.\n- host: myportal.jemena.com.au\n  probed_manually: true\n  note: Customer/trade login wall; / returns 200, /api and /.well-known/openid-configuration return 403.\n- host: poweroutages.jemena.com.au\n  probed_manually: true\n  note: CloudFront distribution, geo-restricted — returns HTTP 403 outside Australia.\n- host: api.jemena.com.au\n  probed_manually: true\n  note: Resolves via Akamai (api.jemena.com.au.edgekey.net);\
  \ returns HTTP 503 on /, /openapi.json, /swagger.json and /health. Internal edge, not a public API.\ndomains:\n- domain: jemena.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jemena/refs/heads/main/security/jemena-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Grid
- Network Distributor
- DER
- Solar
- Smart Metering
- Demand Response
- IEEE 2030.5
---
