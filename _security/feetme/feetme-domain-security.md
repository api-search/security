---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: feetme.fr
  spf: true
hosts:
- cert_expires: Sep 20 12:12:42 2026 GMT
  host: feetme.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feetme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feetme, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Feetme
provider_slug: feetme
slug: feetme-domain-security
source_filename: feetme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feetme.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:12:42 2026 GMT\n  hsts: false\ndomains:\n- domain: feetme.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feetme/refs/heads/main/security/feetme-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Medical Devices
- Digital Health
- Wearables
- Gait Analysis
- Rehabilitation
- Connected Insoles
- MedTech
---
