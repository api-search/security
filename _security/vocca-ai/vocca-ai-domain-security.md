---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vocca.com
  spf: true
hosts:
- cert_expires: Sep 28 21:14:24 2026 GMT
  host: vocca.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vocca Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vocca Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Vocca Ai
provider_slug: vocca-ai
slug: vocca-ai-domain-security
source_filename: vocca-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vocca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:14:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vocca.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vocca-ai/refs/heads/main/security/vocca-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Voice AI
- Conversational AI
- Artificial Intelligence
- Medical
- Patient Communications
- Appointment Booking
- Agents
---
