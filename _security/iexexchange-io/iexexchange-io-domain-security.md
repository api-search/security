---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iexexchange.io
  spf: true
hosts:
- cert_expires: Dec 12 23:11:27 2026 GMT
  host: www.iexexchange.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iexexchange Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IEX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IEX
provider_slug: iexexchange-io
slug: iexexchange-io-domain-security
source_filename: iexexchange-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iexexchange.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:11:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iexexchange.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/iexexchange-io/security/iexexchange-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Stock Market
- Trading
- Market Data
- Technology
---
