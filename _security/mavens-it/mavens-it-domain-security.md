---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mavens.it
  spf: false
hosts:
- cert_expires: Dec 21 10:49:32 2026 GMT
  host: mavens.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MAVENS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MAVENS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: MAVENS
provider_slug: mavens-it
slug: mavens-it-domain-security
source_filename: mavens-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mavens.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 10:49:32 2026 GMT\n  hsts: false\ndomains:\n- domain: mavens.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mavens-it/security/mavens-it-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Security
- Artificial Intelligence
- Code Scanning
- Compliance
- GDPR
- Software-as-a-Service
---
