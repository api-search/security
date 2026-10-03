---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biopk.co.kr
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.biopk.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bioportkorea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bioportkorea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bioportkorea
provider_slug: bioportkorea
slug: bioportkorea-domain-security
source_filename: bioportkorea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biopk.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: biopk.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioportkorea/refs/heads/main/security/bioportkorea-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Food
- Health
- South Korea
- Consumer Goods
---
