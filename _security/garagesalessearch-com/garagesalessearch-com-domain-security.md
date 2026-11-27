---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: garagesalessearch.com
  spf: true
hosts:
- cert_expires: Feb  5 17:06:38 2027 GMT
  host: garagesalessearch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: garagesalessearch-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for garagesalessearch-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: garagesalessearch-com
provider_slug: garagesalessearch-com
slug: garagesalessearch-com-domain-security
source_filename: garagesalessearch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: garagesalessearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 17:06:38 2027 GMT\n  hsts: null\ndomains:\n- domain: garagesalessearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/garagesalessearch-com/security/garagesalessearch-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
