---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lizzyai.com
  spf: true
hosts:
- cert_expires: Oct 16 20:03:06 2026 GMT
  host: lizzyai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lizzyai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lizzyai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lizzyai
provider_slug: lizzyai
slug: lizzyai-domain-security
source_filename: lizzyai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lizzyai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 20:03:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lizzyai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lizzyai/refs/heads/main/security/lizzyai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Legal
- Legal AI
- Generative AI
- Artificial Intelligence
- Legal Technology
- Document Management
- Contract Review
- SaaS
---
