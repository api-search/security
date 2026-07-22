---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: morganlewis.com
  spf: true
hosts:
- cert_expires: Aug 18 16:19:51 2026 GMT
  host: www.morganlewis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morgan Lewis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morgan, Lewis & Bockius LLP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Morgan, Lewis & Bockius LLP
provider_slug: morgan-lewis
slug: morgan-lewis-domain-security
source_filename: morgan-lewis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.morganlewis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:19:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: morganlewis.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morgan-lewis/refs/heads/main/security/morgan-lewis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Law Firm
- Am Law 10
- Employee Benefits
- Fintech
- Intellectual Property
- Mergers And Acquisitions
---
