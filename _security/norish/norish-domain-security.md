---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: norish.dev
  spf: false
hosts:
- cert_expires: Nov 23 11:59:35 2026 GMT
  host: norish.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 17:22:32 2026 GMT
  host: docs.norish.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Norish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Norish, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Norish
provider_slug: norish
slug: norish-domain-security
source_filename: norish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: norish.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 11:59:35 2026 GMT\n  hsts: false\n- host: docs.norish.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:22:32 2026 GMT\n  hsts: false\ndomains:\n- domain: norish.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/norish/refs/heads/main/security/norish-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Recipes
- Meal Planning
- Groceries
- Food
- Self-Hosted
- Open-Source
- Household
- Calendar
- CalDAV
---
