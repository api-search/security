---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucemhealth.com
  spf: true
hosts:
- cert_expires: Oct 15 07:09:18 2026 GMT
  host: lucemhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lucem Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucem Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucem Health
provider_slug: lucem-health
slug: lucem-health-domain-security
source_filename: lucem-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucemhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 07:09:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lucemhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucem-health/refs/heads/main/security/lucem-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Artificial Intelligence
- Machine Learning
- Clinical Decision Support
- Early Disease Detection
- Population Health
- Life Sciences
- Electronic Health Records
---
