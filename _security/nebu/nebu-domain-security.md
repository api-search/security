---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thenebu.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: thenebu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nebu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nebu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nebu
provider_slug: nebu
slug: nebu-domain-security
source_filename: nebu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thenebu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: thenebu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nebu/refs/heads/main/security/nebu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- DevOps
- Cloud
- Artificial Intelligence
- AIOps
- MLOps
- Cloud Management
- Automation
- Cost Optimization
---
