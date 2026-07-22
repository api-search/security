---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "awstrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: propiedades.com
  spf: true
hosts:
- cert_expires: Oct  7 16:20:30 2026 GMT
  host: propiedades.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Okol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Okol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Okol
provider_slug: okol
slug: okol-domain-security
source_filename: okol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: propiedades.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:20:30 2026 GMT\n  hsts: null\ndomains:\n- domain: propiedades.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okol/refs/heads/main/security/okol-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Property
- Marketplace
- Listings
- Mexico
---
