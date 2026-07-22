---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cowbell.insure
  spf: false
hosts:
- cert_expires: Sep 25 17:58:59 2026 GMT
  host: cowbell.insure
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cowbell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cowbell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Cowbell
provider_slug: cowbell
slug: cowbell-domain-security
source_filename: cowbell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cowbell.insure\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:58:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cowbell.insure\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cowbell/refs/heads/main/security/cowbell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cyber Insurance
- Insurance
- InsurTech
- Cybersecurity
- Risk Management
- Risk Assessment
- Continuous Underwriting
- SMB
- Cowbell Factors
- Cyber Liability
- Managed Detection and Response
- Penetration Testing
- Compliance
- Quoting
- Binding
- Brokers
- Agencies
---
