---
description: ''
domains:
- caa:
  - 0 contactemail "security@ozon.ru"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "emsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "emsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ozon.ru
  spf: true
hosts:
- cert_expires: Nov  4 14:46:01 2026 GMT
  host: ozon.ru
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ozonru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OZON.ru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OZON.ru
provider_slug: ozonru
slug: ozonru-domain-security
source_filename: ozonru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ozon.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 14:46:01 2026 GMT\n  hsts: null\ndomains:\n- domain: ozon.ru\n  dnssec: false\n  caa:\n  - 0 contactemail \"security@ozon.ru\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"emsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"emsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozonru/refs/heads/main/security/ozonru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- E-Commerce
- Marketplace
- Seller API
- Russia
- Logistics
---
