---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revlon.com
  spf: true
hosts:
- cert_expires: Oct  3 07:05:33 2026 GMT
  host: www.revlon.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- host: corporate.revlon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Revlon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revlon, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Revlon
provider_slug: revlon
slug: revlon-domain-security
source_filename: revlon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revlon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:05:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: corporate.revlon.com\n  https: false\ndomains:\n- domain: revlon.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revlon/refs/heads/main/security/revlon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Antiperspirant
- Beauty
- Beauty Tools
- Chapter 11
- Color Cosmetics
- Consumer Beauty
- Cosmetics
- Deodorant
- EDI
- Elizabeth Arden
- Fragrance
- Hair Care
- Hair Color
- Licensed Brands
- Mass Market
- Nail Care
- Personal Care
- Post Bankruptcy
- Prestige
- Private Company
- Shopify
- Skin Care
- Supplier Portal
---
