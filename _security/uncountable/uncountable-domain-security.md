---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uncountable.com
  spf: true
hosts:
- cert_expires: Nov  9 15:40:06 2026 GMT
  host: www.uncountable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: app.uncountable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 06:20:43 2026 GMT
  host: www.support.uncountable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uncountable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uncountable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Uncountable
provider_slug: uncountable
slug: uncountable-domain-security
source_filename: uncountable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uncountable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 15:40:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.uncountable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\n- host: www.support.uncountable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:20:43 2026 GMT\n  hsts: false\ndomains:\n- domain: uncountable.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncountable/refs/heads/main/security/uncountable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Laboratory Informatics
- LIMS
- Electronic Lab Notebook
- R&D Data Management
- Product Lifecycle Management
- Quality Management
- Materials Science
- Chemicals
- Artificial Intelligence
- Model Context Protocol
---
