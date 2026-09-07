---
description: 'AbleSky serves HTTPS correctly on a wildcard certificate but the posture is dated: the origin negotiates no higher than TLS 1.2, the certificate is a domain-validated one from a small Chinese CA, and NONE of the four cheap DNS hardening records is published — no DNSSEC, no CAA, no SPF, no DMARC. Absence of a record is valid data, not a probe failure; each was queried directly and returned empty.'
domains:
- caa: []
  caa_evidence: No CAA record — any public CA may issue for this domain. Notable given the wildcard certificate in use.
  dmarc: false
  dmarc_evidence: _dmarc.ablesky.com TXT returns empty.
  dmarc_policy: null
  dnssec: false
  dnssec_evidence: DNSKEY and DS queries both return empty.
  domain: ablesky.com
  hosting: Self-hosted on 222.249.69.20-22 (Beijing), DNS on Alibaba Cloud DNS. No CDN or WAF in front of the origin.
  mx:
  - 10 mailin.ablesky.com
  nameservers:
  - vip1.alidns.com
  - vip2.alidns.com
  spf: false
  spf_evidence: The only TXT record on the apex is a 64-hex verification token ("8d6f7a20...6fccbe"); there is no v=spf1 record, so no sender policy is published for a domain that does accept mail (MX 10 mailin.ablesky.com).
hosts:
- cert_expires: '2026-10-15'
  cert_issuer: C=CN, O=Beijing Xinchacha Credit Management Co., Ltd., CN=Xcc Trust DV SSL CA
  cert_not_before: '2025-10-15'
  cert_san:
  - '*.ablesky.com'
  - ablesky.com
  cert_subject: CN=*.ablesky.com
  cert_validation: DV
  host: www.ablesky.com
  hsts: false
  hsts_max_age: null
  http_status: 200
  https: true
  note: No Strict-Transport-Security header on the 200 response. http:// does 301 to https://, so the redirect is in place; only the HSTS commitment is missing.
  server: nginx/1.22.1
  tls13_evidence: openssl s_client -tls1_3 returns "tlsv1 alert protocol version" (alert 70); the server refuses TLS 1.3 and tops out at TLS 1.2.
  tls13_supported: false
  tls_version: TLSv1.2
- cert_covered_by_san: true
  host: ablesky.com
  hsts: false
  https: true
  note: Apex 301s to https and is covered by the same wildcard certificate.
  tls_version: TLSv1.2
- cert_covered_by_san: true
  host: api.ablesky.com
  hsts: false
  http_status: 403
  https: true
  note: Blanket 403 on every path including "/", from nginx 1.6.0 — a 2014-era build. Recorded as an observation about the deployed banner, not as a vulnerability finding; nothing was probed beyond ordinary GETs.
  server: nginx/1.6.0
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ablesky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AbleSky, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AbleSky
provider_slug: ablesky
slug: ablesky-domain-security
source_filename: ablesky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  Direct TLS/DNS/HTTP probes run on 2026-09-06 against AbleSky's own hosts\n  (openssl s_client for the certificate and protocol ceiling, dig for DNSSEC/CAA/\n  SPF/DMARC, curl for response headers). The shared probe-domain-security.py\n  helper was run twice and reported \"unreachable\" both times — the Beijing origin\n  (222.249.69.0/24) is slow enough from this vantage point to exceed the helper's\n  connect timeout, and an earlier run of it had recorded equityzen.com, the\n  secondary-market listing host that used to sit in apis.yml as Website, which is\n  not an AbleSky property. That stale record has been replaced by these\n  measurements of the real domain.\ndescription: >-\n  AbleSky serves HTTPS correctly on a wildcard certificate but the posture is\n  dated: the origin negotiates no higher than TLS 1.2, the certificate is a\n  domain-validated one from a small Chinese CA, and NONE of the four cheap DNS\n  hardening\
  \ records is published — no DNSSEC, no CAA, no SPF, no DMARC. Absence\n  of a record is valid data, not a probe failure; each was queried directly and\n  returned empty.\nhosts:\n  - host: www.ablesky.com\n    https: true\n    http_status: 200\n    server: nginx/1.22.1\n    tls_version: TLSv1.2\n    tls13_supported: false\n    tls13_evidence: >-\n      openssl s_client -tls1_3 returns \"tlsv1 alert protocol version\" (alert 70);\n      the server refuses TLS 1.3 and tops out at TLS 1.2.\n    cert_subject: CN=*.ablesky.com\n    cert_san:\n      - '*.ablesky.com'\n      - ablesky.com\n    cert_issuer: >-\n      C=CN, O=Beijing Xinchacha Credit Management Co., Ltd.,\n      CN=Xcc Trust DV SSL CA\n    cert_validation: DV\n    cert_not_before: '2025-10-15'\n    cert_expires: '2026-10-15'\n    hsts: false\n    hsts_max_age: null\n    note: >-\n      No Strict-Transport-Security header on the 200 response. http:// does\n      301 to https://, so the redirect is in place; only the HSTS commitment\
  \ is\n      missing.\n  - host: ablesky.com\n    https: true\n    tls_version: TLSv1.2\n    cert_covered_by_san: true\n    hsts: false\n    note: Apex 301s to https and is covered by the same wildcard certificate.\n  - host: api.ablesky.com\n    https: true\n    http_status: 403\n    server: nginx/1.6.0\n    tls_version: TLSv1.2\n    cert_covered_by_san: true\n    hsts: false\n    note: >-\n      Blanket 403 on every path including \"/\", from nginx 1.6.0 — a 2014-era\n      build. Recorded as an observation about the deployed banner, not as a\n      vulnerability finding; nothing was probed beyond ordinary GETs.\ndomains:\n  - domain: ablesky.com\n    dnssec: false\n    dnssec_evidence: DNSKEY and DS queries both return empty.\n    caa: []\n    caa_evidence: >-\n      No CAA record — any public CA may issue for this domain. Notable given the\n      wildcard certificate in use.\n    spf: false\n    spf_evidence: >-\n      The only TXT record on the apex is a 64-hex verification token\n\
  \      (\"8d6f7a20...6fccbe\"); there is no v=spf1 record, so no sender policy is\n      published for a domain that does accept mail (MX 10 mailin.ablesky.com).\n    dmarc: false\n    dmarc_policy: null\n    dmarc_evidence: _dmarc.ablesky.com TXT returns empty.\n    mx:\n      - 10 mailin.ablesky.com\n    nameservers:\n      - vip1.alidns.com\n      - vip2.alidns.com\n    hosting: >-\n      Self-hosted on 222.249.69.20-22 (Beijing), DNS on Alibaba Cloud DNS. No CDN\n      or WAF in front of the origin.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ablesky/refs/heads/main/security/ablesky-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Education
- E-Learning
- Online Courses
- Learning Management
- SaaS
- Training
- K-12
- Live Streaming
- Video
- China
---
