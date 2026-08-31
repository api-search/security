---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: palebluedot.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tokenrouter.com
  spf: false
hosts:
- cert_expires: Oct 19 16:15:03 2026 GMT
  host: www.palebluedot.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 13:07:39 2026 GMT
  host: www.tokenrouter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 03:21:09 2026 GMT
  host: api.tokenrouter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Palebluedotai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PaleBlueDot.AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PaleBlueDot.AI
provider_slug: palebluedotai
slug: palebluedotai-domain-security
source_filename: palebluedotai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.palebluedot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 16:15:03 2026 GMT\n  hsts: false\n- host: www.tokenrouter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:07:39 2026 GMT\n  hsts: false\n- host: api.tokenrouter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 03:21:09 2026 GMT\n  hsts: false\ndomains:\n- domain: palebluedot.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tokenrouter.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palebluedotai/refs/heads/main/security/palebluedotai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Machine-Learning
- Large Language Models
- Inference
- API Gateway
- GPU
- Cloud Computing
- Model Routing
- Compute
- Company
---
