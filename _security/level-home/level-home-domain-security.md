---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: level.co
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: level.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.level.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Level Home Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Level Home, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Level Home
provider_slug: level-home
slug: level-home-domain-security
source_filename: level-home-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: level.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: api.level.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: level.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nx-findings:\n- id: dangling-redirect-levelm-co\n  severity: high\n  summary: >-\n    https://level.co/multifamily/ still issues a 301 to https://levelm.co/ — the domain of the former\n    Level M multifamily business. levelm.co lapsed and was re-registered on 2026-06-11 through NameCheap\n    (Cloudflare nameservers) and now 301-chains to unrelated third-party sites currently serving\n    Indonesian online-gambling SEO content. A Level-branded path on the company's own production domain\n    therefore hands visitors and crawlers to\
  \ content Level does not control.\n  observed: '2026-08-04'\n  evidence:\n  - url: https://level.co/multifamily/\n    http_status: 301\n    location: https://levelm.co/\n    server: Apache/2.4.61 (Craft CMS)\n  - url: https://levelm.co/\n    http_status: 301\n    location: https://patrickmolloyfishing.com/\n    server: cloudflare\n  - source: whois levelm.co\n    creation_date: '2026-06-11'\n    registrar: NameCheap, Inc.\n    note: re-registration date is after the September 2024 ASSA ABLOY transaction, i.e. a dropped-and-recaptured domain\n  remediation: >-\n    Remove or repoint the /multifamily/ redirect (Ambient Property Technologies now serves that audience at\n    https://www.ambientproptech.com/), and audit the Craft CMS redirect table for other rules pointing at\n    domains the company no longer owns.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level-home/refs/heads/main/security/level-home-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- smart-lock
- smart-home
- home-automation
- iot
- access-control
- matter
- thread
- bluetooth-le
- apple-home-key
- consumer-hardware
- multifamily
- proptech
- graphql
---
