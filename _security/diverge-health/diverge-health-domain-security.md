---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: divergehealth.org
  spf: true
hosts:
- cert_expires: Sep 25 13:30:34 2026 GMT
  host: divergehealth.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diverge Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diverge Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diverge Health
provider_slug: diverge-health
slug: diverge-health-domain-security
source_filename: diverge-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divergehealth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:30:34 2026 GMT\n  hsts: false\ndomains:\n- domain: divergehealth.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diverge-health/refs/heads/main/security/diverge-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Value-Based Care
- Medicaid
- Primary Care
- Behavioral Health
---
