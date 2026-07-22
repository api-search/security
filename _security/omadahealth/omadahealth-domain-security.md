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
- cert_expires: Oct  2 15:46:37 2026 GMT
  host: omadahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omadahealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omada Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Omada Health
provider_slug: omadahealth
slug: omadahealth-domain-security
source_filename: omadahealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omadahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: omadahealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omadahealth/refs/heads/main/security/omadahealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Digital Health
- Virtual Care
- Chronic Disease Management
- Diabetes
- Hypertension
- Telehealth
- Health Plans
---
