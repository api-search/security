---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: auctria.com
  spf: true
hosts:
- cert_expires: Mar 31 23:59:59 2027 GMT
  host: www.auctria.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auctria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auctria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Auctria
provider_slug: auctria
slug: auctria-domain-security
source_filename: auctria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auctria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: auctria.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/auctria/security/auctria-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fundraising
- Nonprofit
- SaaS
- Auctions
---
