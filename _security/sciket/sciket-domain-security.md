---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: false
  dnssec: false
  domain: sciket.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: sciket.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sciket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sciket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sciket
provider_slug: sciket
slug: sciket-domain-security
source_filename: sciket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sciket.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sciket.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sciket/refs/heads/main/security/sciket-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- E-commerce
- Marketplace
- Scientific Research
- Laboratory Supplies
- Procurement
- Taiwan
- B2B
---
