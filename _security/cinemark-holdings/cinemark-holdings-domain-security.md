---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cinemark.com
  spf: true
hosts:
- host: www.cinemark.com
  https: false
- cert_expires: Aug 10 12:04:37 2026 GMT
  host: investors.cinemark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cinemark Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cinemark Holdings, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cinemark Holdings
provider_slug: cinemark-holdings
slug: cinemark-holdings-domain-security
source_filename: cinemark-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cinemark.com\n  https: false\n- host: investors.cinemark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 12:04:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cinemark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cinemark-holdings/refs/heads/main/security/cinemark-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cinema
- Entertainment
- Loyalty
- Movie Theaters
- Ticketing
- Fortune 1000
---
