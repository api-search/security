---
description: ''
domains:
- caa: []
  caa_note: No CAA record published for opendorse.com (dig +short CAA returned nothing) — a real absence, not an unread probe.
  dmarc: true
  dmarc_note: DMARC is published but the policy is p=none (monitor only) — no quarantine or reject enforcement.
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none;
  dnssec: true
  domain: opendorse.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: opendorse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.opendorse.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Azure App Service origin behind Azure Front Door; backend for the Opendorse apps, not a published developer API.
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: app.opendorse.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Opendorse web application (client-rendered SPA).
  tls_version: TLSv1.3
- cert_expires: Oct 26 15:24:56 2026 GMT
  host: biz.opendorse.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  note: WordPress marketing site on WP Engine.
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: help.opendorse.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  note: Intercom-hosted help center on an Opendorse CNAME.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendorse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opendorse, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Opendorse
provider_slug: opendorse
slug: opendorse-domain-security
source_filename: opendorse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (probe-domain-security.py), extended 2026-08-26\n  with hand-probed TLS/HSTS for the four additional Opendorse hosts found during STEP 0b contract discovery\n  (api., app., biz., help.)\nhosts:\n- host: opendorse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opendorse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Azure App Service origin behind Azure Front Door; backend for the Opendorse apps, not a published\n    developer API.\n- host: app.opendorse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Opendorse web application (client-rendered SPA).\n\
  - host: biz.opendorse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 15:24:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  note: WordPress marketing site on WP Engine.\n- host: help.opendorse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  note: Intercom-hosted help center on an Opendorse CNAME.\ndomains:\n- domain: opendorse.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  caa_note: No CAA record published for opendorse.com (dig +short CAA returned nothing) — a real absence,\n    not an unread probe.\n  dmarc_record: v=DMARC1; p=none;\n  dmarc_note: DMARC is published but the policy is p=none (monitor only) — no quarantine or reject enforcement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendorse/refs/heads/main/security/opendorse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sports
- Athletes
- Name Image Likeness
- NIL
- Marketplace
- Endorsements
- Social Media
- Compliance
- Higher Education
- Payments
- Marketing
---
