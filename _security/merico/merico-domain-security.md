---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: devinsight.ai
  spf: true
hosts:
- cert_expires: Sep 17 18:27:27 2026 GMT
  host: www.devinsight.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Merico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merico, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Merico
provider_slug: merico
slug: merico-domain-security
source_filename: merico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.devinsight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:27:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: devinsight.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merico/refs/heads/main/security/merico-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Dev Tools
- Engineering Intelligence
- DevOps
- DORA Metrics
- Software Analytics
- Open Source
- Data Platform
---
