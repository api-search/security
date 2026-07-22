---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: speedybrand.io
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: speedybrand.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Speedybrand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpeedyBrand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpeedyBrand
provider_slug: speedybrand
slug: speedybrand-domain-security
source_filename: speedybrand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: speedybrand.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: speedybrand.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speedybrand/refs/heads/main/security/speedybrand-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Enterprise
- SEO
- Content Marketing
- Artificial Intelligence
- Content Generation
- Marketing
- SaaS
---
