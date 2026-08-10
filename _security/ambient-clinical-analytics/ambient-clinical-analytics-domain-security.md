---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ambientclinical.com
  spf: true
hosts:
- cert_expires: Oct 18 10:20:45 2026 GMT
  host: ambientclinical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambient Clinical Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambient Clinical Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ambient Clinical Analytics
provider_slug: ambient-clinical-analytics
slug: ambient-clinical-analytics-domain-security
source_filename: ambient-clinical-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ambientclinical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 10:20:45 2026 GMT\n  hsts: false\ndomains:\n- domain: ambientclinical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambient-clinical-analytics/refs/heads/main/security/ambient-clinical-analytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Clinical Decision Support
- Patient Monitoring
- Sepsis
- Medical Devices
- Electronic Health Records
- Analytics
- Tele-ICU
---
