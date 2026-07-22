---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:devops+security@auto1.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: auto1-group.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.auto1-group.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auto1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auto1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Auto1
provider_slug: auto1
slug: auto1-domain-security
source_filename: auto1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auto1-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: auto1-group.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:devops+security@auto1.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auto1/refs/heads/main/security/auto1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Automotive
- Used Cars
- Marketplace
- Remarketing
- Financing
- Ecommerce
- Europe
---
