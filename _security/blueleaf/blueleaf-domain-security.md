---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blueleaf.com
  spf: true
hosts:
- cert_expires: Sep 26 05:14:55 2026 GMT
  host: blueleaf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blueleaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlueLeaf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BlueLeaf
provider_slug: blueleaf
slug: blueleaf-domain-security
source_filename: blueleaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueleaf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:14:55 2026 GMT\n  hsts: false\ndomains:\n- domain: blueleaf.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueleaf/refs/heads/main/security/blueleaf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wealth Management
- Fintech
- Financial Advisors
- Investment Reporting
- Account Aggregation
- Client Portal
- OAuth
- OpenID Connect
---
