---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: planby.us
  spf: true
hosts:
- cert_expires: Sep  7 03:37:45 2026 GMT
  host: planby.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planby Technologies Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Planby Technologies, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Planby Technologies, Inc.
provider_slug: planby-technologies-inc
slug: planby-technologies-inc-domain-security
source_filename: planby-technologies-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: planby.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 03:37:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: planby.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planby-technologies-inc/refs/heads/main/security/planby-technologies-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Architecture
- Construction
- Rendering
- Visualization
- Consulting
- Seoul
---
