---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chartahealth.com
  spf: true
hosts:
- cert_expires: Oct  7 04:36:21 2026 GMT
  host: www.chartahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charta Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charta Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Charta Health
provider_slug: charta-health
slug: charta-health-domain-security
source_filename: charta-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chartahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:36:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chartahealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charta-health/refs/heads/main/security/charta-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Medical Coding
- Revenue Cycle Management
- Chart Review
- Clinical Documentation
- Risk Adjustment
- Autonomous Coding
- EHR Integration
- Payer Compliance
---
