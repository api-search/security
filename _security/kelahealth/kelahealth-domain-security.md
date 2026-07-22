---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kelahealth.com
  spf: false
hosts:
- cert_expires: Oct 10 10:25:15 2026 GMT
  host: kelahealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kelahealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kelaHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: kelaHealth
provider_slug: kelahealth
slug: kelahealth-domain-security
source_filename: kelahealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kelahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 10:25:15 2026 GMT\n  hsts: null\ndomains:\n- domain: kelahealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kelahealth/refs/heads/main/security/kelahealth-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Surgery
- Artificial Intelligence
- Predictive Analytics
- Perioperative
- Machine Learning
- MedTech
- Patient Risk
- HIPAA
---
