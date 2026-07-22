---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tradedepot.co
  spf: false
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.tradedepot.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradedepot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TradeDepot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TradeDepot
provider_slug: tradedepot
slug: tradedepot-domain-security
source_filename: tradedepot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tradedepot.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tradedepot.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradedepot/refs/heads/main/security/tradedepot-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Applicative Saas
- B2B Commerce
- Retail Distribution
- FMCG
- Ecommerce
- Mobile SDKs
- Africa
- Nigeria
---
