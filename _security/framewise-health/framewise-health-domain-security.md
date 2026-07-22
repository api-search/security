---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: framewisehealth.com
  spf: true
hosts:
- cert_expires: Aug 28 19:10:54 2026 GMT
  host: framewisehealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Framewise Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Framewise Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Framewise Health
provider_slug: framewise-health
slug: framewise-health-domain-security
source_filename: framewise-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: framewisehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:10:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: framewisehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/framewise-health/refs/heads/main/security/framewise-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Patient Engagement
- Patient Education
- FHIR
- EHR Integration
- Health Literacy
- Artificial Intelligence
- HIPAA
- SOC 2
---
