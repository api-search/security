---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tegus.com
  spf: true
- caa: []
  dmarc: true
  dmarc_pct: 10
  dmarc_policy: quarantine
  dnssec: false
  domain: tegus.co
  note: The application domain. DMARC is p=quarantine at pct=10 — only a tenth of failing mail is quarantined — against p=reject on tegus.com. No CAA and no DNSSEC on either.
  spf: true
hosts:
- cert_expires: Sep 12 17:37:17 2026 GMT
  host: www.tegus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:28:05 2026 GMT
  host: auth.tegus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 23:56:48 2026 GMT
  host: app.tegus.co
  hsts: true
  hsts_max_age: 300
  http_status: 403
  https: true
  note: The live Tegus application. HSTS max-age is 300 seconds — two orders of magnitude below the 63072000 used on tegus.com and below the 31536000 an HSTS preload requires. Root returns 403 from Fastly/Varnish with a PerimeterX `_pxhd` cookie (bot challenge).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tegus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tegus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tegus
provider_slug: tegus
slug: tegus-domain-security
source_filename: tegus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tegus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:37:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: auth.tegus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:28:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.tegus.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n  http_status: 403\n  note: >-\n    The live Tegus application. HSTS max-age is 300 seconds — two orders of magnitude\n    below the 63072000 used on tegus.com and below the 31536000 an HSTS preload requires.\n    Root returns 403 from Fastly/Varnish with a PerimeterX `_pxhd` cookie (bot challenge).\ndomains:\n- domain: tegus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tegus.co\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 10\n  note: >-\n    The application domain. DMARC is p=quarantine at pct=10 — only a tenth of failing\n    mail is quarantined — against p=reject on tegus.com. No CAA and no DNSSEC on either.\ndangling_records:\n- host: auth.tegus.co\n  detail: CNAME to a US Auth0 tenant edge; TLS handshake fails.\n- host: help.tegus.co\n  detail: CNAME to tegus.helpjuice.com via CloudFront; sslv3 alert handshake failure.\n  risk: >-\n    A dangling CNAME to a third-party SaaS host is a subdomain-takeover surface if the\n    upstream tenant name is ever released.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tegus/refs/heads/main/security/tegus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Investment Research
- Expert Networks
- Market Intelligence
- Financial Data
- Transcripts
- Private Markets
- Equity Research
- OpenID Connect
- Acquired
---
