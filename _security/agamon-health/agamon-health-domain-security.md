---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agamonhealth.com
  spf: true
hosts:
- cert_expires: Oct  3 21:43:41 2026 GMT
  host: agamonhealth.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agamon Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agamon Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agamon Health
provider_slug: agamon-health
slug: agamon-health-domain-security
source_filename: agamon-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agamonhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: agamonhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agamon-health/refs/heads/main/security/agamon-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Radiology
- Medical Imaging
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Clinical Workflow
- Health Tech
---
