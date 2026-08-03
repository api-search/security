---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: caisgroup.com
  spf: true
hosts:
- cert_expires: Sep 11 16:00:46 2026 GMT
  host: www.caisgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 16:00:46 2026 GMT
  host: mcp.caisgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cais Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CAIS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CAIS
provider_slug: cais
slug: cais-domain-security
source_filename: cais-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:00:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.caisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:00:46 2026 GMT\n  hsts: null\ndomains:\n- domain: caisgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cais/refs/heads/main/security/cais-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Alternative Investments
- Wealth Management
- Financial Services
- Fintech
- Private Markets
- Asset Management
- Structured Products
- Investment Platform
- Artificial Intelligence
---
