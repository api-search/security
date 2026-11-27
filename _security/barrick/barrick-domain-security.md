---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: barrick.com
  spf: true
hosts:
- cert_expires: Dec 23 01:38:02 2026 GMT
  host: www.barrick.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Barrick Mining Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barrick Mining, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Barrick Mining
provider_slug: barrick
slug: barrick-domain-security
source_filename: barrick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barrick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 01:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: barrick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/barrick/security/barrick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Gold
- Resources
- Sustainability
- Investor
---
