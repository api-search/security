---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orghunter.com
  spf: true
hosts:
- cert_expires: Sep 20 08:04:03 2026 GMT
  host: charityapi.orghunter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charity Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charity Search, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Charity Search
provider_slug: charity-search
slug: charity-search-domain-security
source_filename: charity-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charityapi.orghunter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:04:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orghunter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charity-search/refs/heads/main/security/charity-search-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Business
- Public APIs
---
