---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: autotrader.com
  spf: true
hosts:
- cert_expires: Aug 12 17:14:42 2026 GMT
  host: www.autotrader.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autotradercom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoTrader.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AutoTrader.com
provider_slug: autotradercom
slug: autotradercom-domain-security
source_filename: autotradercom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autotrader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:14:42 2026 GMT\n  hsts: false\ndomains:\n- domain: autotrader.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autotradercom/refs/heads/main/security/autotradercom-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Automotive
- Marketplace
- Vehicles
- Cars
- Classifieds
- Dealers
---
