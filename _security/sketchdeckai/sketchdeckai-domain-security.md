---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sketchdeck.ai
  spf: true
hosts:
- cert_expires: Sep 12 22:02:57 2026 GMT
  host: sketchdeck.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sketchdeckai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sketchdeck.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sketchdeck.ai
provider_slug: sketchdeckai
slug: sketchdeckai-domain-security
source_filename: sketchdeckai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sketchdeck.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:02:57 2026 GMT\n  hsts: false\ndomains:\n- domain: sketchdeck.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sketchdeckai/refs/heads/main/security/sketchdeckai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Construction
- Structural Steel
- Steel Estimating
- Takeoff Software
- Bill of Materials
- Artificial Intelligence
- SaaS
---
