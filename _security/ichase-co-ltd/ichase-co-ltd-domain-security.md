---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ichase.io
  spf: true
hosts:
- cert_expires: Sep  6 13:38:13 2026 GMT
  host: ichase.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ichase Co Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iChase Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: iChase Co., Ltd.
provider_slug: ichase-co-ltd
slug: ichase-co-ltd-domain-security
source_filename: ichase-co-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ichase.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:38:13 2026 GMT\n  hsts: false\ndomains:\n- domain: ichase.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ichase-co-ltd/refs/heads/main/security/ichase-co-ltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- AgTech
- Precision Farming
- Livestock
- Poultry
- Biosecurity
- Computer Vision
- Artificial Intelligence
- Animal Health
---
