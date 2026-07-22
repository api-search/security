---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: wenrix.com
  spf: true
hosts:
- cert_expires: Sep 28 08:14:41 2026 GMT
  host: www.wenrix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 16:33:46 2026 GMT
  host: docs.wenrix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wenrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wenrix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Wenrix
provider_slug: wenrix
slug: wenrix-domain-security
source_filename: wenrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wenrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:14:41 2026 GMT\n  hsts: false\n- host: docs.wenrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:33:46 2026 GMT\n  hsts: null\ndomains:\n- domain: wenrix.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wenrix/refs/heads/main/security/wenrix-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Travel
- Airlines
- Booking
- Artificial Intelligence
- Automation
- Pricing
- MCP
- Model Context Protocol
---
