---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: foodhealthcollective.org
  spf: true
hosts:
- cert_expires: Oct 19 11:38:22 2026 GMT
  host: foodhealthcollective.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ahara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AHARA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AHARA
provider_slug: ahara
slug: ahara-domain-security
source_filename: ahara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foodhealthcollective.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 11:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foodhealthcollective.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahara/refs/heads/main/security/ahara-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Nutrition
- Personalized Nutrition
- Digital Health
- Food as Medicine
- Preventive Health
- Consumer Health
- Employer Benefits
- Health Plans
- Mobile App
- Wellness
---
