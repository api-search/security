---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iplogs.com
  spf: false
hosts:
- cert_expires: Sep 10 05:33:48 2026 GMT
  host: iplogs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iplogs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPLogs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: IPLogs
provider_slug: iplogs
slug: iplogs-domain-security
source_filename: iplogs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iplogs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: iplogs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iplogs/refs/heads/main/security/iplogs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Security
- Public APIs
---
