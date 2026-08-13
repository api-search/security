---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: storytellit.com
  note: The primary brand domain carries only Google site-verification TXT records — no SPF, no DMARC, no CAA, no DNSSEC.
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: likeablelocal.com
  note: The legacy brand domain still publishes SPF (Google Workspace) while the current brand domain does not, and neither publishes DMARC. Mail authentication regressed across the rebrand.
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Sep 13 06:08:51 2026 GMT
  host: storytellit.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: api.storytellit.com
  hsts: false
  https: true
  note: Production API host. Serves the application backend; no HSTS header on any response, so a downgrade window exists on first contact.
- cert_expires: Oct 24 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M01
  host: app.storytellit.com
  hsts: false
  https: true
  note: Login-gated application host behind CloudFront; no HSTS header.
kind: domain-security
layout: security
method: probed
name: Likeable Local Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Likeable Local, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Likeable Local
provider_slug: likeable-local
slug: likeable-local-domain-security
source_filename: likeable-local-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml hosts, extended by hand to the production API host and the\n  application host discovered in the 2026-08-12 round\nhosts:\n- host: storytellit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 06:08:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.storytellit.com\n  https: true\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  cert_issuer: Amazon RSA 2048 M04\n  hsts: false\n  note: >-\n    Production API host. Serves the application backend; no HSTS header on any response, so a\n    downgrade window exists on first contact.\n- host: app.storytellit.com\n  https: true\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  cert_issuer: Amazon RSA 2048 M01\n  hsts: false\n  note: Login-gated application host behind CloudFront; no HSTS header.\ndomains:\n- domain: storytellit.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    The primary brand\
  \ domain carries only Google site-verification TXT records — no SPF, no DMARC,\n    no CAA, no DNSSEC.\n- domain: likeablelocal.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: false\n  note: >-\n    The legacy brand domain still publishes SPF (Google Workspace) while the current brand domain\n    does not, and neither publishes DMARC. Mail authentication regressed across the rebrand.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/likeable-local/refs/heads/main/security/likeable-local-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Social Media
- Marketing
- Social Media Management
- Advertising
- Small Business
- Agencies
- SaaS
---
