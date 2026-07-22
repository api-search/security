---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: universalcorp.com
  spf: true
hosts:
- cert_expires: Nov  4 12:49:59 2026 GMT
  host: www.universalcorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universal Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Universal Corporation
provider_slug: universal
slug: universal-domain-security
source_filename: universal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.universalcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 12:49:59 2026 GMT\n  hsts: false\ndomains:\n- domain: universalcorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universal/refs/heads/main/security/universal-domain-security.yml
summary_line: TLSv1.3
tags:
- Agriculture
- Tobacco
- Supply Chain
- Commodity Trading
- Global Trade
- Fortune 1000
---
