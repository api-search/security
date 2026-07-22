---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: habi.co
  spf: true
hosts:
- cert_expires: Aug 18 21:39:51 2026 GMT
  host: habi.co
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Habi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Habi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Habi
provider_slug: habi
slug: habi-domain-security
source_filename: habi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: habi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:39:51 2026 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: habi.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habi/refs/heads/main/security/habi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Real Estate
- iBuyer
- Colombia
- Mexico
- Mortgage
- Home Buying
---
