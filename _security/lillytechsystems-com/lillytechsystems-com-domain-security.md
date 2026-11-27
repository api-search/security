---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lillytechsystems.com
  spf: true
hosts:
- cert_expires: Dec 29 03:50:20 2026 GMT
  host: lillytechsystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lilly Tech Systems, LLC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lilly Tech Systems, LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lilly Tech Systems, LLC
provider_slug: lillytechsystems-com
slug: lillytechsystems-com-domain-security
source_filename: lillytechsystems-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lillytechsystems.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 03:50:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lillytechsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lillytechsystems-com/security/lillytechsystems-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Artificial Intelligence
- IT Services
- Consulting
- Software
- Education
---
