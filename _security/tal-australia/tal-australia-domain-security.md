---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tal.com.au
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.tal.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 11:50:10 2026 GMT
  host: login.talpartner.tal.com.au
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.grouphq.tal.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tal Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TAL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TAL
provider_slug: tal-australia
slug: tal-australia-domain-security
source_filename: tal-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tal.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: login.talpartner.tal.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 11:50:10 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: www.grouphq.tal.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tal.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tal-australia/refs/heads/main/security/tal-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Life Insurance
- Income Protection
- Group Insurance
- Superannuation
- Underwriting
- Claims
- Carrier
- Embedded Insurance
- Partner Gated
- No Public API
- OpenID Connect
- GraphQL
- Identity
---
