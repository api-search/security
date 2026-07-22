---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: niahealth.ai
  spf: true
hosts:
- cert_expires: Sep 22 10:29:12 2026 GMT
  host: www.niahealth.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nia Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nia Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nia Health
provider_slug: nia-health
slug: nia-health-domain-security
source_filename: nia-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.niahealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:29:12 2026 GMT\n  hsts: false\ndomains:\n- domain: niahealth.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nia-health/refs/heads/main/security/nia-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Digital Health
- Medical Device
- Dermatology
- Patient Engagement
- Mobile App
- Berlin
---
