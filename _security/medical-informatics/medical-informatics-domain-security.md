---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sickbay.com
  spf: true
hosts:
- cert_expires: Sep 30 08:48:54 2026 GMT
  host: sickbay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medical Informatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medical Informatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medical Informatics
provider_slug: medical-informatics
slug: medical-informatics-domain-security
source_filename: medical-informatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sickbay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:48:54 2026 GMT\n  hsts: false\ndomains:\n- domain: sickbay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medical-informatics/refs/heads/main/security/medical-informatics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Patient Monitoring
- Clinical Informatics
- Predictive Analytics
- Remote Patient Monitoring
- Digital Health
---
