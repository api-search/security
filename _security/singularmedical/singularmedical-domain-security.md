---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: singularmedical.net
  spf: true
hosts:
- cert_expires: Aug 23 15:32:12 2026 GMT
  host: singularmedical.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Singularmedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Singular Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Singular Medical
provider_slug: singularmedical
slug: singularmedical-domain-security
source_filename: singularmedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: singularmedical.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:32:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: singularmedical.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singularmedical/refs/heads/main/security/singularmedical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- MedTech
- Healthcare
- Cardiology
- Cardiac Rhythm Management
- Implantable Devices
- China
---
