---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cheddarup.com
  spf: true
hosts:
- cert_expires: Sep 30 17:01:44 2026 GMT
  host: cheddarup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cheddar Up Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cheddar Up, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cheddar Up
provider_slug: cheddar-up
slug: cheddar-up-domain-security
source_filename: cheddar-up-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cheddarup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:01:44 2026 GMT\n  hsts: null\ndomains:\n- domain: cheddarup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheddar-up/refs/heads/main/security/cheddar-up-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Group Payments
- Fundraising
- Nonprofits
- Schools
- Forms
- Fintech
- Payment Collection
---
