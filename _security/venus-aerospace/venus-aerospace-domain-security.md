---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: venusaero.com
  spf: true
hosts:
- cert_expires: Oct 30 19:33:03 2026 GMT
  host: www.venusaero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Venus Aerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Venus Aerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Venus Aerospace
provider_slug: venus-aerospace
slug: venus-aerospace-domain-security
source_filename: venus-aerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.venusaero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: venusaero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venus-aerospace/refs/heads/main/security/venus-aerospace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aerospace
- Propulsion
- Hypersonics
- Rocket Engines
- Defense
- Space
---
