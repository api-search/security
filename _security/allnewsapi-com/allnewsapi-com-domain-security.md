---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: allnewsapi.com
  spf: true
hosts:
- cert_expires: Jan 10 02:17:39 2027 GMT
  host: allnewsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allnewsapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for allnewsapi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: allnewsapi-com
provider_slug: allnewsapi-com
slug: allnewsapi-com-domain-security
source_filename: allnewsapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allnewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 02:17:39 2027 GMT\n  hsts: false\ndomains:\n- domain: allnewsapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/allnewsapi-com/security/allnewsapi-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- News
- API
- Data
- Media
- Aggregation
- Company
---
