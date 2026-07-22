---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: polyai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: poly.ai
  spf: true
hosts:
- host: www.polyai.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Sep 23 18:22:32 2026 GMT
  host: docs.poly.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.us.poly.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Polyai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polyai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Polyai
provider_slug: polyai
slug: polyai-domain-security
source_filename: polyai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polyai.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: docs.poly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:22:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us.poly.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: polyai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: poly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyai/refs/heads/main/security/polyai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Conversational AI
- Voice AI
- Customer Service
- Contact Center
- Agents
- Speech Recognition
- Text to Speech
- Webhooks
- Enterprise
---
