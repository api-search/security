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
- cert_expires: Oct 12 03:43:16 2026 GMT
  host: www.cinemark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 08:02:23 2026 GMT
  host: investors.cinemark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cinemark Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cinemark Holdings, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cinemark Holdings
provider_slug: cinemark-holdings
slug: cinemark-holdings-domain-security
source_filename: cinemark-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cinemark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:43:16 2026 GMT\n  hsts: false\n- host: investors.cinemark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:02:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cinemark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
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
