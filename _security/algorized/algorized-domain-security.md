---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: algorized.com
  spf: true
hosts:
- cert_expires: Dec  4 16:44:49 2026 GMT
  host: www.algorized.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Algorized Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Algorized, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Algorized
provider_slug: algorized
slug: algorized-domain-security
source_filename: algorized-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.algorized.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 16:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: algorized.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algorized/refs/heads/main/security/algorized-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Edge Computing
- Robotics
- Safety
---
