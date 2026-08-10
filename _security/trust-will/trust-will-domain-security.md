---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trustandwill.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: trustandwill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.trustandwill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: live application API host; responds with JSON errors, no public documentation
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: app.trustandwill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trust Will Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trust & Will, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Trust & Will
provider_slug: trust-will
slug: trust-will-domain-security
source_filename: trust-will-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustandwill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trustandwill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: live application API host; responds with JSON errors, no public documentation\n- host: app.trustandwill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trustandwill.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trust-will/refs/heads/main/security/trust-will-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Estate Planning
- Wills And Trusts
- Probate
- Legal
- Financial Services
- Wealth Management
- Fintech
---
