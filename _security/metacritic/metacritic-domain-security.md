---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metacritic.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fabricdata.com
  spf: true
hosts:
- cert_expires: Sep 27 00:01:34 2026 GMT
  host: www.metacritic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: developer.origin.fabricdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.origin.fabricdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metacritic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metacritic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Metacritic
provider_slug: metacritic
slug: metacritic-domain-security
source_filename: metacritic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metacritic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:01:34 2026 GMT\n  hsts: false\n- host: developer.origin.fabricdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.origin.fabricdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: metacritic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fabricdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metacritic/refs/heads/main/security/metacritic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Reviews
- Metascore
- Games
- Movies
- Television
- Music
- Review Aggregator
- Critic Scores
- User Scores
---
