---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fritz.ai
  spf: true
hosts:
- cert_expires: Aug 24 14:19:38 2026 GMT
  host: fritz.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fritzai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fritz.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fritz.ai
provider_slug: fritzai
slug: fritzai-domain-security
source_filename: fritzai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fritz.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:19:38 2026 GMT\n  hsts: false\ndomains:\n- domain: fritz.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fritzai/refs/heads/main/security/fritzai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Machine Learning
- Artificial Intelligence
- Mobile
- On-Device ML
- Developer Tools
- SDKs
- Defunct
---
