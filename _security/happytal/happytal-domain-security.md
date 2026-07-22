---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: happytal.com
  spf: true
hosts:
- cert_expires: Sep 27 04:19:09 2026 GMT
  host: www.happytal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Happytal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Happytal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Happytal
provider_slug: happytal
slug: happytal-domain-security
source_filename: happytal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.happytal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:19:09 2026 GMT\n  hsts: false\ndomains:\n- domain: happytal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happytal/refs/heads/main/security/happytal-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Healthcare
- Health
- France
- Concierge
- Marketplace
- Elder Care
- Patient Experience
- HealthTech
---
