---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ai2robotics.com
  spf: true
hosts:
- cert_expires: Nov  9 18:07:59 2026 GMT
  host: ai2robotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 18:07:59 2026 GMT
  host: docs.ai2robotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ai2Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ai²robotics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ai²robotics
provider_slug: ai2robotics
slug: ai2robotics-domain-security
source_filename: ai2robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai2robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 18:07:59 2026 GMT\n  hsts: false\n- host: docs.ai2robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 18:07:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ai2robotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai2robotics/refs/heads/main/security/ai2robotics-domain-security.yml
summary_line: TLSv1.3
tags:
- Robotics
- AI
- AGI
- Manufacturing
- Shenzhen
---
