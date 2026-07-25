---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cboe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: livevol.com
  spf: true
hosts:
- cert_expires: Oct 19 00:39:46 2026 GMT
  host: www.cboe.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:31:28 2026 GMT
  host: api.livevol.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 15:29:26 2026 GMT
  host: cdn.cboe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cboe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cboe Global Markets, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cboe Global Markets
provider_slug: cboe
slug: cboe-domain-security
source_filename: cboe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cboe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 00:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.livevol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:31:28 2026 GMT\n  hsts: false\n- host: cdn.cboe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:29:26 2026 GMT\n  hsts: null\ndomains:\n- domain: cboe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: livevol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cboe/refs/heads/main/security/cboe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Market Data
- Options
- Equities
- Derivatives
- Volatility
- Financial Markets
- Exchanges
- Trading
---
