---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prolonlife.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: l-nutrahealth.com
  spf: true
hosts:
- cert_expires: Nov 10 04:42:02 2026 GMT
  host: prolonlife.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 03:09:01 2026 GMT
  host: l-nutrahealth.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 03:45:32 2026 GMT
  host: l-nutraprofessional.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: L Nutra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for L-Nutra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: L-Nutra
provider_slug: l-nutra
slug: l-nutra-domain-security
source_filename: l-nutra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prolonlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 04:42:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: l-nutrahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 03:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: l-nutraprofessional.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:45:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: prolonlife.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: l-nutrahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/l-nutra/refs/heads/main/security/l-nutra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nutrition
- Health
- Longevity
- Consumer Products
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
