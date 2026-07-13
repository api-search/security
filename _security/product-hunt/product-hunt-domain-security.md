---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: producthunt.com
  spf: true
hosts:
- cert_expires: Oct  6 01:11:14 2026 GMT
  host: api.producthunt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Product Hunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Product Hunt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Product Hunt
provider_slug: product-hunt
slug: product-hunt-domain-security
source_filename: product-hunt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.producthunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:11:14 2026 GMT\n  hsts: null\ndomains:\n- domain: producthunt.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/product-hunt/refs/heads/main/security/product-hunt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Product Discovery
- Startups
- Tech Products
- Maker Community
---
