---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cuspai.com
  spf: false
hosts:
- cert_expires: Sep 30 01:10:20 2026 GMT
  host: www.cuspai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: redirects (301) to canonical https://www.cusp.ai/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cuspai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuspai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cuspai
provider_slug: cuspai
slug: cuspai-domain-security
source_filename: cuspai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cuspai.com\n  note: redirects (301) to canonical https://www.cusp.ai/\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:10:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cuspai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuspai/refs/heads/main/security/cuspai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Materials Discovery
- Materials Science
- Deep Learning
- Carbon Capture
- Enterprise
---
