---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leaftfoods.com
  spf: true
hosts:
- cert_expires: Sep  2 00:49:02 2026 GMT
  host: www.leaftfoods.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leaftfoods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leaft Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Leaft Foods
provider_slug: leaftfoods
slug: leaftfoods-domain-security
source_filename: leaftfoods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leaftfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: leaftfoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaftfoods/refs/heads/main/security/leaftfoods-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food
- AgTech
- Alternative Protein
- Ingredients
- Pet Nutrition
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- New Zealand
---
