---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aisensum.com
  spf: true
hosts:
- cert_expires: Sep 20 16:04:20 2026 GMT
  host: aisensum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aisensum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AiSensum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AiSensum
provider_slug: aisensum
slug: aisensum-domain-security
source_filename: aisensum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aisensum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:04:20 2026 GMT\n  hsts: false\ndomains:\n- domain: aisensum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aisensum/refs/heads/main/security/aisensum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Retail
- Food and Beverage
- Hospitality
- Customer Experience
- Enterprise Software
- Southeast Asia
---
