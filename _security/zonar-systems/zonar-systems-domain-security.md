---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zonar.com
  spf: true
hosts:
- cert_expires: Nov 17 18:58:24 2026 GMT
  host: www.zonar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zonar Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zonar Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Zonar Systems
provider_slug: zonar-systems
slug: zonar-systems-domain-security
source_filename: zonar-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zonar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 18:58:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zonar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zonar-systems/refs/heads/main/security/zonar-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fleet Management
- Telematics
- Safety
- Compliance
---
