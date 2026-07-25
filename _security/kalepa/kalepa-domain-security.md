---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kalepa.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kalepa.co
  note: In responsible-disclosure scope.
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: kalepainsurance.com
  note: In responsible-disclosure scope. No SPF and no DMARC record.
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: kalepa.io
  note: 'In responsible-disclosure scope. Weakest posture of the four: unsigned, no CAA, no SPF, no DMARC.'
  spf: false
hosts:
- cert_expires: Aug 25 15:49:03 2026 GMT
  host: kalepa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 00:29:07 2026 GMT
  host: www.kalepa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.kalepa.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: 'Production API host. A CloudFront function returns a bodyless 404 (x-cache: FunctionGeneratedResponse) for every unmatched path, which is why every documentation and discovery probe uniformly 404s.'
  security_headers:
    referrer-policy: strict-origin-when-cross-origin
    x-content-type-options: nosniff
    x-frame-options: DENY
    x-xss-protection: 1; mode=block
  server: CloudFront
  tls_version: TLSv1.3
- cert_expires: Oct 13 20:47:19 2026 GMT
  host: copilot.kalepa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Copilot application front end. 307-redirects to https://api.kalepa.com/auth/login?frontend_redirect_url=... — the customer login wall.
  server: Vercel
  tls_version: TLSv1.3
- cert_expires: Oct 11 06:06:13 2026 GMT
  host: status.kalepa.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  note: Better Stack hosted status page.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kalepa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kalepa, probed live across 5 host(s) and 4 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kalepa
provider_slug: kalepa
slug: kalepa-domain-security
source_filename: kalepa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of the apis.yml hosts plus the production API host,\n  the Copilot application host, the status host, and the three additional\n  domains named in the responsible-disclosure scope\nhosts:\n- host: kalepa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:49:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.kalepa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:29:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kalepa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: CloudFront\n  security_headers:\n    x-frame-options: DENY\n    x-content-type-options: nosniff\n    x-xss-protection: 1; mode=block\n    referrer-policy: strict-origin-when-cross-origin\n  note: >-\n    Production API host.\
  \ A CloudFront function returns a bodyless 404\n    (x-cache: FunctionGeneratedResponse) for every unmatched path, which is why\n    every documentation and discovery probe uniformly 404s.\n- host: copilot.kalepa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:47:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: Vercel\n  note: >-\n    Copilot application front end. 307-redirects to\n    https://api.kalepa.com/auth/login?frontend_redirect_url=... — the customer\n    login wall.\n- host: status.kalepa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 06:06:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  note: Better Stack hosted status page.\ndomains:\n- domain: kalepa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kalepa.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: In responsible-disclosure scope.\n- domain: kalepainsurance.com\n\
  \  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n  note: In responsible-disclosure scope. No SPF and no DMARC record.\n- domain: kalepa.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    In responsible-disclosure scope. Weakest posture of the four: unsigned, no\n    CAA, no SPF, no DMARC.\nsummary:\n  tls: All five hosts negotiate TLSv1.3.\n  hsts: All five hosts set HSTS; api.kalepa.com is includeSubDomains + preload.\n  caa: No CAA records on any of the four registrable domains.\n  dnssec: Signed on kalepa.com, kalepa.co and kalepainsurance.com; unsigned on kalepa.io.\n  email_auth: >-\n    SPF + DMARC (quarantine) on kalepa.com and kalepa.co; neither on\n    kalepainsurance.com or kalepa.io, both of which are in disclosure scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalepa/refs/heads/main/security/kalepa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- United States
- Insurtech
- Underwriting
- Property and Casualty
- Commercial Insurance
- Artificial Intelligence
- ACORD
- Partner Gated
- No Public API
---
