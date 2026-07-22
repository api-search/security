---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: konnhomes.com
  spf: true
hosts:
- cert_expires: Oct  5 15:42:12 2026 GMT
  host: konnhomes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Konn Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konn Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Konn Technologies
provider_slug: konn-technologies
slug: konn-technologies-domain-security
source_filename: konn-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konnhomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:42:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: konnhomes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konn-technologies/refs/heads/main/security/konn-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Architecture
- Real Estate
- Construction Technology
- PropTech
- Home Design
- Jordan
- Middle East
---
