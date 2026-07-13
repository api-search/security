---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: newsdata.io
  spf: true
hosts:
- cert_expires: Feb  2 05:37:42 2027 GMT
  host: newsdata.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newsdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewsData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NewsData
provider_slug: newsdata
slug: newsdata-domain-security
source_filename: newsdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newsdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 05:37:42 2027 GMT\n  hsts: false\ndomains:\n- domain: newsdata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newsdata/refs/heads/main/security/newsdata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Media
- Search
- Content
---
