---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bluebirds.com
  spf: true
hosts:
- cert_expires: Sep 26 14:05:35 2026 GMT
  host: bluebirds.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluebirds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluebirds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bluebirds
provider_slug: bluebirds
slug: bluebirds-domain-security
source_filename: bluebirds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluebirds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:05:35 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: bluebirds.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluebirds/refs/heads/main/security/bluebirds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales
- Go-To-Market
- Prospecting
- Sales Intelligence
- Outbound Sales
- Artificial Intelligence
- Software-as-a-Service
- Lead Generation
---
