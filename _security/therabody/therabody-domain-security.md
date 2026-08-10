---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: therabody.com
  spf: true
hosts:
- cert_expires: Oct 13 10:25:02 2026 GMT
  host: www.therabody.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 10:35:01 2026 GMT
  host: account.therabody.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Therabody Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Therabody, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Therabody
provider_slug: therabody
slug: therabody-domain-security
source_filename: therabody-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.therabody.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: account.therabody.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:35:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: therabody.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: Scoped to Therabody-controlled hosts. shopify.dev appears in apis.yml only as\n  the humanURL for the Shopify-documented Storefront GraphQL API and is not a Therabody\n  domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/therabody/refs/heads/main/security/therabody-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wellness
- Health
- Consumer Products
- E-Commerce
- Retail
- Shopify
- Agentic Commerce
- Model Context Protocol
- GraphQL
- Universal Commerce Protocol
---
