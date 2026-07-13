---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wto.org
  spf: true
hosts:
- cert_expires: Aug 21 12:12:17 2026 GMT
  host: www.wto.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: apiportal.wto.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.wto.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WTO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WTO
provider_slug: wto
slug: wto-domain-security
source_filename: wto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wto.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:12:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apiportal.wto.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wto.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wto.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wto/refs/heads/main/security/wto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- World Trade
- Trade Statistics
- Tariffs
- Trade Flows
- Trade Policy
- International Trade
- Global Trade
- Merchandise Trade
- Services Trade
- Market Access
- Non-Tariff Measures
- Quantitative Restrictions
- Dispute Settlement
- Trade Notifications
- Open Data
---
