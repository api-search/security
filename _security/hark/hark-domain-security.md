---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hark.com
  spf: true
hosts:
- cert_expires: Oct  2 08:36:34 2026 GMT
  host: hark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hark
provider_slug: hark
slug: hark-domain-security
source_filename: hark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:36:34 2026 GMT\n  hsts: null\ndomains:\n- domain: hark.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hark/refs/heads/main/security/hark-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Foundation Models
- Agents
- Consumer Hardware
- Consumer Electronics
- Devices
- Assistants
- Pre-Product
---
