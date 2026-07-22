---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chefsforseniors.com
  spf: true
hosts:
- cert_expires: Aug 27 20:02:45 2026 GMT
  host: chefsforseniors.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chefs For Seniors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chefs for Seniors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chefs for Seniors
provider_slug: chefs-for-seniors
slug: chefs-for-seniors-domain-security
source_filename: chefs-for-seniors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chefsforseniors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:02:45 2026 GMT\n  hsts: false\ndomains:\n- domain: chefsforseniors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chefs-for-seniors/refs/heads/main/security/chefs-for-seniors-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Senior Care
- Meal Preparation
- Personal Chef
- Food Service
- Nutrition
- Home Care
- Franchise
---
