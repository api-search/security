---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: false
  domain: nacelle.com
  spf: true
hosts:
- cert_expires: Sep 13 19:15:48 2026 GMT
  host: nacelle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:01:32 2026 GMT
  host: docs.nacelle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nacelle Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nacelle, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nacelle
provider_slug: nacelle-com
slug: nacelle-com-domain-security
source_filename: nacelle-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:15:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:01:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nacelle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacelle-com/refs/heads/main/security/nacelle-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Commerce
- Ecommerce
- Headless Commerce
- Composable Commerce
- Storefront
- Personalization
- AI Personalization
- Product Recommendations
- Data Orchestration
- GraphQL
- Shopify
- Contentful
- Sanity
---
