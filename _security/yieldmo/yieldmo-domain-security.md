---
api_specs:
- filename: yieldmo-dcs-mcp-openapi.json
  format: json
  label: Yieldmo DCS Reporting API
  slug: yieldmo-dcs-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-dcs-mcp-openapi.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "symantec.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yieldmo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prebid.org
  spf: true
hosts:
- cert_expires: Nov  9 15:35:04 2026 GMT
  host: yieldmo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: ads.yieldmo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 08:30:18 2026 GMT
  host: docs.prebid.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.yieldmo.com
  hsts: false
  https: true
  note: API host carrying the MCP server and DCS reporting API. Probed manually 2026-08-12 — probe-domain-security.py did not enumerate it. No Strict-Transport-Security header on the AWS API Gateway responses.
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:01:38 2026 GMT
  host: apps.yieldmo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: YMax console/login host. Probed manually 2026-08-12. The only Yieldmo host observed serving HSTS.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yieldmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yieldmo, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yieldmo
provider_slug: yieldmo
slug: yieldmo-domain-security
source_filename: yieldmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yieldmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 15:35:04 2026 GMT\n  hsts: false\n- host: ads.yieldmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\n- host: docs.prebid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:30:18 2026 GMT\n  hsts: false\n- host: api.yieldmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n  note: API host carrying the MCP server and DCS reporting API. Probed manually 2026-08-12 — probe-domain-security.py\n    did not enumerate it. No Strict-Transport-Security header on the AWS API Gateway responses.\n- host: apps.yieldmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:01:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: YMax console/login host. Probed\
  \ manually 2026-08-12. The only Yieldmo host observed serving HSTS.\ndomains:\n- domain: yieldmo.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"symantec.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: prebid.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-addendum:\n  manual_hosts_added: 2026-08-12 — api.yieldmo.com and apps.yieldmo.com probed by hand (openssl s_client\n    + curl -I); both discovered this enrichment round and not enumerated by the script.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/security/yieldmo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Programmatic
- Native Advertising
- Ad Exchange
- Publisher Monetization
- Header Bidding
- Contextual Targeting
- Ad Formats
- Supply Side Platform
- SSP
- Campaign Reporting
- Attention Analytics
- MCP
- Prebid
- AdTech
---
