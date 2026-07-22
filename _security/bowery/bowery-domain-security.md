---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boweryfarming.com
  spf: false
hosts:
- cert_expires: Sep 10 16:04:05 2026 GMT
  host: boweryfarming.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bowery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bowery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bowery
provider_slug: bowery
slug: bowery-domain-security
source_filename: bowery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boweryfarming.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:04:05 2026 GMT\n  hsts: false\ndomains:\n- domain: boweryfarming.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bowery/refs/heads/main/security/bowery-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AgTech
- Vertical Farming
- Indoor Farming
- Controlled Environment Agriculture
- Agriculture
- Food
- Sustainability
---
