---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ketone.com
  spf: true
hosts:
- cert_expires: Sep 12 05:26:03 2026 GMT
  host: ketone.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hvmn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HVMN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HVMN
provider_slug: hvmn
slug: hvmn-domain-security
source_filename: hvmn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ketone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:26:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: ketone.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hvmn/refs/heads/main/security/hvmn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Nutrition
- Ketones
- Supplements
- E-Commerce
- Shopify
- Agentic Commerce
- Consumer
- MCP
---
