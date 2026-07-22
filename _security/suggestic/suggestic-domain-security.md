---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: suggestic.com
  spf: true
hosts:
- cert_expires: Oct  7 12:52:45 2026 GMT
  host: suggestic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 01:26:08 2026 GMT
  host: docs.suggestic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:16:44 2026 GMT
  host: production.suggestic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suggestic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suggestic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Suggestic
provider_slug: suggestic
slug: suggestic-domain-security
source_filename: suggestic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suggestic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:52:45 2026 GMT\n  hsts: false\n- host: docs.suggestic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:26:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: production.suggestic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:16:44 2026 GMT\n  hsts: null\ndomains:\n- domain: suggestic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suggestic/refs/heads/main/security/suggestic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nutrition
- Health
- Meal Planning
- Recipes
- Food
- GraphQL
- Personalization
- Wellness
- Telehealth
- Artificial Intelligence
---
