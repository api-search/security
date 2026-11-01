---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lungpacer.com
  spf: true
hosts:
- cert_expires: Jan  6 21:37:33 2027 GMT
  host: www.lungpacer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lungpacer Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lungpacer Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lungpacer Medical
provider_slug: lungpacer-medical
slug: lungpacer-medical-domain-security
source_filename: lungpacer-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lungpacer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 21:37:33 2027 GMT\n  hsts: false\ndomains:\n- domain: lungpacer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lungpacer-medical/security/lungpacer-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Diaphragm Pacing
- Neurostimulation
- Ventilator Weaning
- Critical Care
- Medical Devices
---
