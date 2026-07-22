---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: canbridgepharma.com
  spf: true
hosts:
- cert_expires: Sep  8 10:16:18 2026 GMT
  host: canbridgepharma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canbridgepharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CANbridge Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CANbridge Pharmaceuticals
provider_slug: canbridgepharma
slug: canbridgepharma-domain-security
source_filename: canbridgepharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canbridgepharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:16:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canbridgepharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canbridgepharma/refs/heads/main/security/canbridgepharma-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Rare Disease
- Healthcare
- Life Sciences
- Gene Therapy
- Oncology
---
