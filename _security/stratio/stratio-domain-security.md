---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stratio.ai
  spf: true
hosts:
- cert_expires: Nov 21 07:17:56 2026 GMT
  host: stratio.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stratio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stratio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stratio
provider_slug: stratio
slug: stratio-domain-security
source_filename: stratio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stratio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 07:17:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stratio.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/stratio/security/stratio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Decision-Intelligence
- Regulated-Enterprises
- Data-Governance
---
