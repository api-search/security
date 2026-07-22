---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: outlier.org
  spf: true
hosts:
- cert_expires: Oct 15 04:13:11 2026 GMT
  host: www.outlier.org
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outlier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outlier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Outlier
provider_slug: outlier
slug: outlier-domain-security
source_filename: outlier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.outlier.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:13:11 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: outlier.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outlier/refs/heads/main/security/outlier-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Education
- Online Learning
- Dual Enrollment
- E-Commerce
- Shopify
- Agent Commerce
- MCP
---
