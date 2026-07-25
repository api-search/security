---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iexcloud.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: iexapis.com
  spf: false
hosts:
- cert_expires: Oct 16 03:27:23 2026 GMT
  host: www.iexcloud.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: iexcloud.io
  https: false
- host: cloud.iexapis.com
  https: false
kind: domain-security
layout: security
method: probed
name: Iex Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IEX Cloud, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: IEX Cloud
provider_slug: iex-cloud
slug: iex-cloud-domain-security
source_filename: iex-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnotes: >-\n  IEX Cloud sunset 2024-08-31. The iexcloud.io domain has lapsed out of IEX\n  Group's control - www.iexcloud.io now serves a Namecheap domain-parking lander,\n  so its TLS certificate and DNS posture below describe the parking service, not\n  IEX Group. cloud.iexapis.com (former API host) no longer answers HTTPS.\nhosts:\n- host: www.iexcloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:27:23 2026 GMT\n  hsts: false\n- host: iexcloud.io\n  https: false\n- host: cloud.iexapis.com\n  https: false\ndomains:\n- domain: iexcloud.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: iexapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iex-cloud/refs/heads/main/security/iex-cloud-domain-security.yml
summary_line: TLSv1.3
tags:
- Fintech
- Market Data
- Stocks
- Reference
- Sunset
- Historical
---
