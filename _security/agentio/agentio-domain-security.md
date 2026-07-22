---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentio.com
  spf: true
hosts:
- cert_expires: Oct  4 03:33:02 2026 GMT
  host: agentio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agentio
provider_slug: agentio
slug: agentio-domain-security
source_filename: agentio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:33:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentio/refs/heads/main/security/agentio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Adtech
- Advertising
- Creator Economy
- Influencer Marketing
- Marketing
- Artificial Intelligence
- YouTube
---
