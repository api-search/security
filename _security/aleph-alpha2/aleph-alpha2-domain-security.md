---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aleph-alpha.com
  spf: true
hosts:
- cert_expires: Sep  2 04:14:01 2026 GMT
  host: aleph-alpha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:16:25 2026 GMT
  host: docs.aleph-alpha.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:59:15 2026 GMT
  host: api.aleph-alpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aleph Alpha2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aleph Alpha2, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aleph Alpha2
provider_slug: aleph-alpha2
slug: aleph-alpha2-domain-security
source_filename: aleph-alpha2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aleph-alpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 04:14:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.aleph-alpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:16:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.aleph-alpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:59:15 2026 GMT\n  hsts: null\ndomains:\n- domain: aleph-alpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha2/refs/heads/main/security/aleph-alpha2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Large Language Models
- Machine Learning
- Generative AI
- Sovereign AI
- Inference API
- Embeddings
- Europe
- Germany
- Enterprise AI
---
