---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adsmom.com
  spf: true
hosts:
- cert_expires: Oct  2 08:10:53 2026 GMT
  host: adsmom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adsmom Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adsmom Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adsmom Inc.
provider_slug: adsmom-inc
slug: adsmom-inc-domain-security
source_filename: adsmom-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adsmom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:10:53 2026 GMT\n  hsts: false\ndomains:\n- domain: adsmom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adsmom-inc/refs/heads/main/security/adsmom-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Ad Intelligence
- Competitive Intelligence
- Marketing
- AI
- MCP
- SaaS
---
