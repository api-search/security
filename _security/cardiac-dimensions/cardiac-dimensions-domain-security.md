---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cardiacdimensions.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: cardiacdimensions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardiac Dimensions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardiac Dimensions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cardiac Dimensions
provider_slug: cardiac-dimensions
slug: cardiac-dimensions-domain-security
source_filename: cardiac-dimensions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardiacdimensions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cardiacdimensions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiac-dimensions/refs/heads/main/security/cardiac-dimensions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Cardiology
- Heart Failure
- Structural Heart
- Transcatheter
- Healthcare
- Medical Technology
---
