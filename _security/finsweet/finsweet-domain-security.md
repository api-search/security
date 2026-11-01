---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finsweet.com
  spf: true
hosts:
- cert_expires: Jan  7 19:52:13 2027 GMT
  host: finsweet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Finsweet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finsweet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Finsweet
provider_slug: finsweet
slug: finsweet-domain-security
source_filename: finsweet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finsweet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 19:52:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finsweet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/finsweet/security/finsweet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Webflow
- Development
- Design
- Agency
- SaaS
---
