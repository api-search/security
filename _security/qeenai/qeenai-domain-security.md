---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qeen.ai
  spf: true
hosts:
- cert_expires: Sep 22 11:45:44 2026 GMT
  host: qeen.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qeenai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qeen.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qeen.AI
provider_slug: qeenai
slug: qeenai-domain-security
source_filename: qeenai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qeen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:45:44 2026 GMT\n  hsts: false\ndomains:\n- domain: qeen.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qeenai/refs/heads/main/security/qeenai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Marketing
- Ecommerce
- Advertising
- MENA
---
