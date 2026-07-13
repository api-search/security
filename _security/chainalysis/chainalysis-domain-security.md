---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:cory.watson@chainalysis.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chainalysis.com
  spf: true
hosts:
- cert_expires: Sep 23 04:33:48 2026 GMT
  host: www.chainalysis.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:48:56 2026 GMT
  host: go.chainalysis.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 00:13:09 2026 GMT
  host: public.chainalysis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chainalysis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chainalysis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chainalysis
provider_slug: chainalysis
slug: chainalysis-domain-security
source_filename: chainalysis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chainalysis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: go.chainalysis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:48:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: public.chainalysis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 00:13:09 2026 GMT\n  hsts: null\ndomains:\n- domain: chainalysis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:cory.watson@chainalysis.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainalysis/refs/heads/main/security/chainalysis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- AML
- KYT
- Sanctions
- Investigations
- Blockchain Analytics
- Risk
- Crypto
---
