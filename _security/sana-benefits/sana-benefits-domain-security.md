---
description: ''
domains:
- caa: []
  caa_note: No CAA record is published, so any CA may issue for this domain.
  dmarc: true
  dmarc_note: p=quarantine but pct=10 — only 10% of failing mail is quarantined — and sp=none leaves subdomains unprotected. Partial enforcement, not full.
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=10; rua=mailto:8b5dad9de7d6.a@dmarcinput.com; ruf=mailto:8b5dad9de7d6.f@dmarcinput.com; sp=none; fo=1
  dnssec: false
  domain: sanabenefits.com
  spf: true
hosts:
- cert_expires: Oct  5 04:45:32 2026 GMT
  host: www.sanabenefits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: WordPress marketing site
  tls_version: TLSv1.3
- cert_expires: Aug 27 14:32:34 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  cert_subject: CN=sanabenefits.com
  host: secure.sanabenefits.com
  hsts: false
  https: true
  note: Login-walled Rails application host serving the member/employer/broker dashboards. Probed manually on 2026-07-25 (it is not an apis.yml baseURL, so the automated sweep did not reach it). No Strict-Transport-Security header is returned on the HTTP/2 200 response — a real gap on the host that carries authenticated PHI-adjacent sessions.
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:43:24 2026 GMT
  cert_subject: CN=help.sanabenefits.com
  host: help.sanabenefits.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Zendesk help center; returns 302 to the hosted help center and 403 to automated fetches
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sana Benefits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sana Benefits, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sana Benefits
provider_slug: sana-benefits
slug: sana-benefits-domain-security
source_filename: sana-benefits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sanabenefits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:45:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: WordPress marketing site\n- host: secure.sanabenefits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:32:34 2026 GMT\n  cert_subject: CN=sanabenefits.com\n  cert_issuer: Google Trust Services (WE1)\n  hsts: false\n  server: cloudflare\n  note: >-\n    Login-walled Rails application host serving the member/employer/broker\n    dashboards. Probed manually on 2026-07-25 (it is not an apis.yml baseURL, so\n    the automated sweep did not reach it). No Strict-Transport-Security header is\n    returned on the HTTP/2 200 response — a real gap on the host that carries\n    authenticated PHI-adjacent sessions.\n- host: help.sanabenefits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ Aug 25 23:43:24 2026 GMT\n  cert_subject: CN=help.sanabenefits.com\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Zendesk help center; returns 302 to the hosted help center and 403 to automated fetches\ndomains:\n- domain: sanabenefits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; pct=10; rua=mailto:8b5dad9de7d6.a@dmarcinput.com; ruf=mailto:8b5dad9de7d6.f@dmarcinput.com; sp=none; fo=1'\n  dmarc_note: >-\n    p=quarantine but pct=10 — only 10% of failing mail is quarantined — and\n    sp=none leaves subdomains unprotected. Partial enforcement, not full.\n  caa_note: No CAA record is published, so any CA may issue for this domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana-benefits/refs/heads/main/security/sana-benefits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Health Insurance
- Employee Benefits
- Benefits Administration
- Small Business
- Level-Funded Plans
- Insurtech
- Broker
- Virtual Primary Care
---
