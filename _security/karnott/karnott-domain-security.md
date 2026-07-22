---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: karnott.fr
  spf: true
hosts:
- cert_expires: Sep 14 05:02:37 2026 GMT
  host: www.karnott.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karnott Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karnott, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Karnott
provider_slug: karnott
slug: karnott-domain-security
source_filename: karnott-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.karnott.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:02:37 2026 GMT\n  hsts: null\ndomains:\n- domain: karnott.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karnott/refs/heads/main/security/karnott-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food & Agritech
- Agriculture
- IoT
- Equipment Management
- Fleet Management
- Viticulture
- Farm Management
- France
---
