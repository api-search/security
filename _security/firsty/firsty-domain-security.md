---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: firsty.app
  spf: true
hosts:
- cert_expires: Aug 24 23:02:44 2026 GMT
  host: firsty.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firsty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firsty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Firsty
provider_slug: firsty
slug: firsty-domain-security
source_filename: firsty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firsty.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:02:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firsty.app\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firsty/refs/heads/main/security/firsty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- eSIM
- Mobile
- Connectivity
- Telecommunications
- Travel
- Roaming
- Data
- Consumer
---
