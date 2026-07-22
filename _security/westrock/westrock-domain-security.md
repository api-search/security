---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: westrock.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.westrock.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Westrock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WestRock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WestRock
provider_slug: westrock
slug: westrock-domain-security
source_filename: westrock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westrock.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: westrock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westrock/refs/heads/main/security/westrock-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Packaging
- Paper
- Containers
- Manufacturing
- Supply Chain
- Fortune 500
---
