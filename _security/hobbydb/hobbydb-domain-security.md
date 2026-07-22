---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hobbydb.com
  spf: true
hosts:
- cert_expires: Sep 15 10:01:47 2026 GMT
  host: hobbydb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hobbydb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hobbyDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: hobbyDB
provider_slug: hobbydb
slug: hobbydb-domain-security
source_filename: hobbydb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hobbydb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:01:47 2026 GMT\n  hsts: false\ndomains:\n- domain: hobbydb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hobbydb/refs/heads/main/security/hobbydb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Collectibles
- Marketplace
- Database
- Collections
- Ecommerce
- Auctions
- Community
---
