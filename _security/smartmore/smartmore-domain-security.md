---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smartmore.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: global.smartmore.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartmore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartMore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SmartMore
provider_slug: smartmore
slug: smartmore-domain-security
source_filename: smartmore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.smartmore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smartmore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartmore/refs/heads/main/security/smartmore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Industrial AI
- Machine Vision
- Computer Vision
- Smart Manufacturing
- Quality Inspection
- Deep Learning
- Industrial Automation
- Edge AI
- Hardware
---
