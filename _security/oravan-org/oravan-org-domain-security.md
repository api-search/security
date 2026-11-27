---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oravan.org
  spf: true
hosts:
- cert_expires: Dec 23 22:20:43 2026 GMT
  host: oravan.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oravan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oravan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oravan
provider_slug: oravan-org
slug: oravan-org-domain-security
source_filename: oravan-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oravan.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 22:20:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oravan.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oravan-org/security/oravan-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Civic Tech
- Non-Profit
- PrivacyFocused
- Open Data
---
