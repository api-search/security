---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leantaas.com
  spf: true
hosts:
- cert_expires: Oct 14 12:35:14 2026 GMT
  host: leantaas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leantaas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeanTaaS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LeanTaaS
provider_slug: leantaas
slug: leantaas-domain-security
source_filename: leantaas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leantaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:35:14 2026 GMT\n  hsts: false\ndomains:\n- domain: leantaas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leantaas/refs/heads/main/security/leantaas-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Systems
- Hospital Operations
- Capacity Management
- Artificial Intelligence
- Machine Learning
- Predictive Analytics
- Scheduling
- SaaS
---
