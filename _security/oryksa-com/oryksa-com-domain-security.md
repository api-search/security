---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oryksa.com
  spf: true
hosts:
- cert_expires: Jan 19 08:44:14 2027 GMT
  host: oryksa.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ORYKSA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ORYKSA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ORYKSA
provider_slug: oryksa-com
slug: oryksa-com-domain-security
source_filename: oryksa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oryksa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 08:44:14 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: oryksa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/oryksa-com/security/oryksa-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automation
- Sales
- Customer Service
- Software-as-a-Service
---
