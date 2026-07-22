---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: praxhealth.com
  spf: true
hosts:
- cert_expires: Sep 10 18:05:21 2026 GMT
  host: www.praxhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prax Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prax Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prax Health
provider_slug: prax-health
slug: prax-health-domain-security
source_filename: prax-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.praxhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:05:21 2026 GMT\n  hsts: false\ndomains:\n- domain: praxhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prax-health/refs/heads/main/security/prax-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Technology
- Nurse Practitioners
- Independent Practice
- Practice Management
- EHR
- Medical Billing
- Insurance Credentialing
- Compliance
---
