---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cytora.com
  spf: true
hosts:
- cert_expires: Aug 29 04:47:24 2026 GMT
  host: cytora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:56:19 2026 GMT
  host: docs.cytora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.cytora.com
  https: false
  note: TCP 443 accepts but the TLS handshake is reset by peer for anonymous clients
- cert_expires: Sep 20 23:30:52 2026 GMT
  host: auth.cytora.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: uwp.cytora.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 06:03:07 2026 GMT
  host: status.cytora.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 20:45:58 2026 GMT
  host: trust.cytora.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cytora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cytora, probed live across 7 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cytora
provider_slug: cytora
slug: cytora-domain-security
source_filename: cytora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cytora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:47:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cytora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:56:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cytora.com\n  https: false\n  note: TCP 443 accepts but the TLS handshake is reset by peer for anonymous clients\n- host: auth.cytora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: uwp.cytora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: status.cytora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug\
  \ 31 06:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: trust.cytora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:45:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: cytora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cytora/refs/heads/main/security/cytora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Commercial Insurance
- Underwriting
- Claims
- Risk Data
- Property and Casualty
- Reinsurance
- Brokers
- Submission Intake
- Document AI
---
