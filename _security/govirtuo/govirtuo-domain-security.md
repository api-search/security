---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: govirtuo.com
  spf: true
hosts:
- cert_expires: Sep  1 10:11:49 2026 GMT
  host: www.govirtuo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Govirtuo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtuo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Virtuo
provider_slug: govirtuo
slug: govirtuo-domain-security
source_filename: govirtuo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govirtuo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:11:49 2026 GMT\n  hsts: false\ndomains:\n- domain: govirtuo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govirtuo/refs/heads/main/security/govirtuo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Car Rental
- Mobility
- Travel
- Transportation
- Automotive
- Fleet
- Mobile App
---
