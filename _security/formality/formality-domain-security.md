---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formality.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.formality.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 14:10:51 2026 GMT
  host: help.formality.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: app.eu1.formality.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: EU/Ireland application + API host; carries the /api/v1/{workspaceId} surface.
  tls_version: TLSv1.3
- cert_expires: Oct  1 05:10:55 2026 GMT
  host: app.fr1.formality.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: France/Scaleway sovereign application + API host.
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: auth.eu1.formality.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: Login host the Swagger UI redirects to.
  tls_version: TLSv1.3
- cert_expires: Sep 28 20:10:03 2026 GMT
  host: status.formality.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Formality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formality, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Formality
provider_slug: formality
slug: formality-domain-security
source_filename: formality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.formality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n- host: help.formality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:10:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.eu1.formality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: EU/Ireland application + API host; carries the /api/v1/{workspaceId} surface.\n- host: app.fr1.formality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:10:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: France/Scaleway sovereign application + API host.\n- host: auth.eu1.formality.com\n  https: true\n\
  \  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Login host the Swagger UI redirects to.\n- host: status.formality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: formality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnotes: >-\n  The four regional/app hosts were added by hand from the same live TLS + HTTP HEAD\n  probes on 2026-08-17 because apis[].baseURL is templated\n  (https://app.eu1.formality.com/api/v1/{workspaceId}) and the automated prober\n  skips templated bases. Findings worth noting: the application, auth and API hosts\n  all set a strong HSTS policy (max-age 63072000, includeSubDomains, preload), but\n  the marketing origin www.formality.com now returns NO HSTS header at all after its\n  migration to Framer — a regression\
  \ against the 2026-07-19 probe, which recorded\n  hsts: true / max-age 31536000. The registrable domain still has no DNSSEC and no\n  CAA records, and DMARC remains at p=none, so a spoofed formality.com mail is not\n  rejected.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formality/refs/heads/main/security/formality-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai/Ml
- Legal
- Contract Management
- Document Management
- Asset Intelligence
- Compliance
- SaaS
---
