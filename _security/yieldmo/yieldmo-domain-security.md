---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "symantec.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
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
- cert_expires: Sep 10 16:26:29 2026 GMT
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
kind: domain-security
layout: security
method: probed
name: Yieldmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yieldmo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yieldmo
provider_slug: yieldmo
slug: yieldmo-domain-security
source_filename: yieldmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yieldmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:26:29 2026 GMT\n  hsts: false\n- host: ads.yieldmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\n- host: docs.prebid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:30:18 2026 GMT\n  hsts: false\ndomains:\n- domain: yieldmo.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"symantec.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: prebid.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/security/yieldmo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Programmatic
- Native Advertising
- Ad Exchange
- Publisher Monetization
- Header Bidding
- Contextual Targeting
- Ad Formats
- Supply-Side Platform
- SSP
---
