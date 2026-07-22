---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vitesseautomation.com
  spf: true
hosts:
- cert_expires: Oct 19 09:03:42 2026 GMT
  host: vitesseautomation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vitesse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vitesse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vitesse
provider_slug: vitesse
slug: vitesse-domain-security
source_filename: vitesse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vitesseautomation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 09:03:42 2026 GMT\n  hsts: false\ndomains:\n- domain: vitesseautomation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitesse/refs/heads/main/security/vitesse-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Physical AI
- Industrial Automation
- Operational Technology
- Manufacturing
- IoT
- Edge Computing
- SCADA
- PLC
- Robotics
- Cybersecurity
- Interoperability
---
