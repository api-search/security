---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: layer2solutions.com
  spf: true
hosts:
- cert_expires: Dec 14 05:12:24 2026 GMT
  host: layer2solutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Layer2Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Layer 2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Layer 2
provider_slug: layer2solutions
slug: layer2solutions-domain-security
source_filename: layer2solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layer2solutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 05:12:24 2026 GMT\n  hsts: false\ndomains:\n- domain: layer2solutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/layer2solutions/security/layer2solutions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Integration
- File Synchronization
- Microsoft Cloud
- Office 365
---
