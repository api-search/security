---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 90
  dmarc_policy: quarantine
  dmarc_rua: true
  dmarc_subdomain_policy: none
  dnssec: false
  domain: comulate.com
  spf: true
  spf_policy: -all
  spf_record: v=spf1 include:dc-aa8e722993._spfm.comulate.com -all
hosts:
- cert_expires: Oct 14 17:36:58 2026 GMT
  host: comulate.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: marketing website
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: app.comulate.com
  hsts: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  role: hosted application
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: api.comulate.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_preload: false
  https: true
  note: Returns 401 on every path except the root health check. Response carries a full helmet-style header set — CSP default-src 'self', COEP require-corp, COOP same-origin, CORP same-origin, X-Frame-Options DENY, X-Content-Type-Options nosniff, Referrer-Policy no-referrer, X-Permitted-Cross-Domain-Policies none.
  role: production API host (auth-gated)
  tls_version: TLSv1.3
- cert_expires: Oct 11 17:14:46 2026 GMT
  host: trust.comulate.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63113904
  hsts_preload: true
  https: true
  role: status page (Better Stack hosted)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comulate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comulate, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Comulate
provider_slug: comulate
slug: comulate-domain-security
source_filename: comulate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Comulate host discovered in apis.yml + DNS\nhosts:\n- host: comulate.com\n  role: marketing website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:36:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: false\n- host: app.comulate.com\n  role: hosted application\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_preload: true\n- host: api.comulate.com\n  role: production API host (auth-gated)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  note: >-\n    Returns 401 on every path except the root health check. Response carries a full\n    helmet-style header set — CSP default-src 'self', COEP require-corp, COOP\n    same-origin, CORP same-origin, X-Frame-Options\
  \ DENY, X-Content-Type-Options nosniff,\n    Referrer-Policy no-referrer, X-Permitted-Cross-Domain-Policies none.\n- host: trust.comulate.com\n  role: status page (Better Stack hosted)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:14:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: comulate.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  spf_record: v=spf1 include:dc-aa8e722993._spfm.comulate.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: none\n  dmarc_pct: 90\n  dmarc_rua: true\nfindings:\n- HSTS is enabled on all four hosts; app and trust are preload-eligible, comulate.com and\n  api.comulate.com are not.\n- No CAA records are published, so any CA may issue for comulate.com.\n- DNSSEC is not enabled (no DS record).\n- SPF is a hard fail (-all), which is the strong setting.\n- DMARC is p=quarantine at pct=90 with sp=none, so subdomains\
  \ are unprotected and 10\n  percent of failing mail is unhandled — short of a full p=reject posture.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comulate/refs/heads/main/security/comulate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Accounting
- Reconciliation
- Automation
- Revenue Intelligence
- Fintech
- Insurance Brokers
---
