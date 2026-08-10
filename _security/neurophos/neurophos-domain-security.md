---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: neurophos.com
  spf: true
hosts:
- cert_expires: Sep  5 12:51:51 2026 GMT
  host: www.neurophos.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neurophos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neurophos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Neurophos
provider_slug: neurophos
slug: neurophos-domain-security
source_filename: neurophos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neurophos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 12:51:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: neurophos.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurophos/refs/heads/main/security/neurophos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- photonics
- optical-computing
- ai-inference
- ai-accelerators
- semiconductors
- metamaterials
- data-center
- deep-tech
- mcp
---
