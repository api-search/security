---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: producthunt.com
  spf: true
hosts:
- cert_expires: Oct  6 01:11:14 2026 GMT
  host: www.producthunt.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:11:14 2026 GMT
  host: api.producthunt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Producthunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Product Hunt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Product Hunt
provider_slug: producthunt
slug: producthunt-domain-security
source_filename: producthunt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.producthunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.producthunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:11:14 2026 GMT\n  hsts: null\ndomains:\n- domain: producthunt.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/producthunt/refs/heads/main/security/producthunt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Product Discovery
- GraphQL
- Community
- Products
- Startups
- Launches
- Voting
- Tech
---
