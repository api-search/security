---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: braincorp.com
  spf: true
hosts:
- cert_expires: Nov 24 19:12:20 2026 GMT
  host: www.braincorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Braincorporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braincorporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Braincorporation
provider_slug: braincorporation
slug: braincorporation-domain-security
source_filename: braincorporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.braincorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 19:12:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: braincorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braincorporation/refs/heads/main/security/braincorporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Robotics
- Autonomous
- Enterprise
- Platform
---
