---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: weismarkets.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: streamcollab.com
  spf: true
hosts:
- cert_expires: Sep 26 20:31:53 2026 GMT
  host: www.weismarkets.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 01:17:57 2026 GMT
  host: weismarkets.streamcollab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weis Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for weis-markets, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: weis-markets
provider_slug: weis-markets
slug: weis-markets-domain-security
source_filename: weis-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weismarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:31:53 2026 GMT\n  hsts: null\n- host: weismarkets.streamcollab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:17:57 2026 GMT\n  hsts: null\ndomains:\n- domain: weismarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: streamcollab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weis-markets/refs/heads/main/security/weis-markets-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 1000
---
