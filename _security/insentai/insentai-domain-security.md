---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: insent.ai
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: insent.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insentai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insent.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Insent.ai
provider_slug: insentai
slug: insentai-domain-security
source_filename: insentai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: insent.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insentai/refs/heads/main/security/insentai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Conversational Marketing
- Chat
- Sales Engagement
- MarTech
- B2B
- Acquired
---
