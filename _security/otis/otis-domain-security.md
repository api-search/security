---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: withotis.com
  spf: false
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: withotis.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Otis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Otis
provider_slug: otis
slug: otis-domain-security
source_filename: otis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withotis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: withotis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otis/refs/heads/main/security/otis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Investing
- Alternative Assets
- Collectibles
- Wealth Management
- Acquired
---
