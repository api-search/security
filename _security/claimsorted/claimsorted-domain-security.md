---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: claimsorted.com
  spf: true
hosts:
- cert_expires: Sep 11 18:42:35 2026 GMT
  host: www.claimsorted.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Claimsorted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClaimSorted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClaimSorted
provider_slug: claimsorted
slug: claimsorted-domain-security
source_filename: claimsorted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.claimsorted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:42:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: claimsorted.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claimsorted/refs/heads/main/security/claimsorted-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Claims
- Claims Management
- Third-Party Administrator
- Fraud Detection
---
