---
description: ''
domains:
- caa:
  - digicert.com
  - letsencrypt.org
  - pki.goog
  - ssl.com
  - comodoca.com
  - microsoft.com
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: start.gg
  spf: true
  spf_record: v=spf1 include:amazonses.com include:servers.mcsv.net include:_spf.google.com -all
hosts:
- host: api.start.gg
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- host: developer.start.gg
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
- host: www.start.gg
  hsts: false
  https: true
kind: domain-security
layout: security
method: probed
name: Smashgg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smashgg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smashgg
provider_slug: smashgg
slug: smashgg-domain-security
source_filename: smashgg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: TLS handshake + HTTP HEAD + dig (probed 2026-07-21)\nhosts:\n  - host: api.start.gg\n    https: true\n    tls_version: TLSv1.3\n    hsts: true\n    hsts_max_age: 15724800\n    hsts_include_subdomains: true\n  - host: developer.start.gg\n    https: true\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: false\n  - host: www.start.gg\n    https: true\n    hsts: false\ndomains:\n  - domain: start.gg\n    dnssec: false\n    caa:\n      - digicert.com\n      - letsencrypt.org\n      - pki.goog\n      - ssl.com\n      - comodoca.com\n      - microsoft.com\n    spf: true\n    spf_record: 'v=spf1 include:amazonses.com include:servers.mcsv.net include:_spf.google.com -all'\n    dmarc: true\n    dmarc_policy: reject\nnotes: >-\n  start.gg (smash.gg's successor; smash.gg 301-redirects to www.start.gg) is a\n  Microsoft property - the CAA record authorizes microsoft.com as a certificate\n  issuer. DMARC is enforced\
  \ (p=reject). DNSSEC is not enabled.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smashgg/refs/heads/main/security/smashgg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Esports
- Gaming
- Tournaments
- GraphQL
- Events
- Developer API
---
