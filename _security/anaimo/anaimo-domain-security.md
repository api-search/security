---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anaimo.com
  spf: true
hosts:
- cert_expires: Dec 13 16:12:06 2026 GMT
  host: anaimo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anaimo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anaimo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anaimo
provider_slug: anaimo
slug: anaimo-domain-security
source_filename: anaimo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anaimo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 16:12:06 2026 GMT\n  hsts: false\ndomains:\n- domain: anaimo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anaimo/refs/heads/main/security/anaimo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Automation
- VirtualAssistant
- Retail
---
