---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: marketaux.com
  spf: true
hosts:
- cert_expires: Oct  4 04:37:20 2026 GMT
  host: www.marketaux.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketaux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketAux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: MarketAux
provider_slug: marketaux
slug: marketaux-domain-security
source_filename: marketaux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marketaux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:37:20 2026 GMT\n  hsts: false\ndomains:\n- domain: marketaux.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketaux/refs/heads/main/security/marketaux-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- News
- Public APIs
---
