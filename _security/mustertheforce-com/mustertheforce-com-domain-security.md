---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mustertheforce.com
  spf: false
hosts:
- cert_expires: Dec 30 20:35:20 2026 GMT
  host: mustertheforce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MustertheForce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MustertheForce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: MustertheForce
provider_slug: mustertheforce-com
slug: mustertheforce-com-domain-security
source_filename: mustertheforce-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mustertheforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 20:35:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mustertheforce.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mustertheforce-com/security/mustertheforce-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Salesforce
- Marketplace
- Freelancing
- Hiring
- GigPlatform
---
