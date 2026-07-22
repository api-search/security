---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: omadahealth.com
  spf: true
hosts:
- cert_expires: Sep 30 07:16:35 2026 GMT
  host: www.omadahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omada Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omada Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Omada Health
provider_slug: omada-health
slug: omada-health-domain-security
source_filename: omada-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omadahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: omadahealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omada-health/refs/heads/main/security/omada-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Digital Health
- Virtual Care
- Chronic Disease Management
- Diabetes
- Hypertension
- Healthcare
- HIPAA
- Telehealth
---
