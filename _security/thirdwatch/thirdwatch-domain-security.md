---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thirdwatch.app
  spf: true
hosts:
- cert_expires: Dec 12 05:52:51 2026 GMT
  host: thirdwatch.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thirdwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThirdWatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ThirdWatch
provider_slug: thirdwatch
slug: thirdwatch-domain-security
source_filename: thirdwatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thirdwatch.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 05:52:51 2026 GMT\n  hsts: false\ndomains:\n- domain: thirdwatch.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/thirdwatch/security/thirdwatch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Monitoring
- Authentication
- JWT
- OpenAPI
- Alerting
- Performance Dashboard
- Multi‑organization
- Anomaly Detection
---
