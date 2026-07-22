---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seasonshare.com
  spf: true
hosts:
- cert_expires: Aug  2 20:13:20 2026 GMT
  host: seasonshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Season Share Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Season Share, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Season Share
provider_slug: season-share
slug: season-share-domain-security
source_filename: season-share-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seasonshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 20:13:20 2026 GMT\n  hsts: false\ndomains:\n- domain: seasonshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/season-share/refs/heads/main/security/season-share-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ticketing
- Sports
- Entertainment
- Events
- Fan Engagement
- SaaS
---
