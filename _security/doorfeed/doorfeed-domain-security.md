---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doorfeed.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: doorfeed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doorfeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoorFeed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DoorFeed
provider_slug: doorfeed
slug: doorfeed-domain-security
source_filename: doorfeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doorfeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: doorfeed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doorfeed/refs/heads/main/security/doorfeed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- PropTech
- Real Estate
- Investment
- Residential
- Property Data
- France
- United Kingdom
---
