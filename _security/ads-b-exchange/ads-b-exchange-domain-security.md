---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adsbexchange.com
  spf: true
hosts:
- cert_expires: Sep 19 20:12:12 2026 GMT
  host: www.adsbexchange.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ads B Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADS-B Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ADS-B Exchange
provider_slug: ads-b-exchange
slug: ads-b-exchange-domain-security
source_filename: ads-b-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adsbexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:12:12 2026 GMT\n  hsts: false\ndomains:\n- domain: adsbexchange.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ads-b-exchange/refs/heads/main/security/ads-b-exchange-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
