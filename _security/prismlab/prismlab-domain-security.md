---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prismlab.cn
  spf: false
hosts:
- cert_expires: Oct  1 18:01:50 2026 GMT
  host: prismlab.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Prismlab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prismlab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prismlab
provider_slug: prismlab
slug: prismlab-domain-security
source_filename: prismlab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prismlab.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 18:01:50 2026 GMT\n  hsts: false\ndomains:\n- domain: prismlab.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prismlab/refs/heads/main/security/prismlab-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- 3D Printing
- Additive Manufacturing
- Hardware
- Manufacturing
- Dental
- Medical Devices
- Industrial
---
