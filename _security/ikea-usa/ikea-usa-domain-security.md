---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ikea.com
  spf: true
hosts:
- cert_expires: Oct  3 14:53:21 2026 GMT
  host: www.ikea.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ikea Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IKEA U.S., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IKEA U.S.
provider_slug: ikea-usa
slug: ikea-usa-domain-security
source_filename: ikea-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ikea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:53:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ikea.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikea-usa/refs/heads/main/security/ikea-usa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B
- Big-Box
- Buy Back
- Click And Collect
- Delivery
- E-commerce
- Furniture
- Home Furnishings
- Home Smart
- IKEA Family
- Kitchen
- Loyalty
- Mobile App
- Planning Tools
- Retail
- Smart Home
- Sustainability
- Swedish
---
