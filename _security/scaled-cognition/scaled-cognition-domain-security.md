---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scaledcognition.com
  spf: true
hosts:
- cert_expires: Oct 25 13:02:42 2026 GMT
  host: www.scaledcognition.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: api.scaledcognition.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scaled Cognition Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scaled Cognition, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scaled Cognition
provider_slug: scaled-cognition
slug: scaled-cognition-domain-security
source_filename: scaled-cognition-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scaledcognition.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:02:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.scaledcognition.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: scaledcognition.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scaled-cognition/refs/heads/main/security/scaled-cognition-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Agents
- Large Language Models
- Customer Experience
- Contact Center
- Conversational AI
- Voice
- Enterprise Software
- Machine-Learning
- Company
---
