---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rssboard.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
hosts:
- cert_expires: Oct  2 15:16:56 2026 GMT
  host: www.rssboard.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: datatracker.ietf.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:21:33 2026 GMT
  host: www.jsonfeed.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RSS
provider_slug: rss
slug: rss-domain-security
source_filename: rss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rssboard.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 15:16:56 2026 GMT\n  hsts: false\n- host: datatracker.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: www.jsonfeed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:21:33 2026 GMT\n  hsts: false\ndomains:\n- domain: rssboard.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rss/refs/heads/main/security/rss-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Syndication
- RSS
- Atom
- JSON Feed
- OPML
- Content
- XML
- Specification
- Standard
---
