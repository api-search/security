---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elevationspine.com
  spf: true
hosts:
- cert_expires: Sep 28 12:55:23 2026 GMT
  host: www.elevationspine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elevation Spine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elevation Spine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elevation Spine
provider_slug: elevation-spine
slug: elevation-spine-domain-security
source_filename: elevation-spine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elevationspine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:55:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elevationspine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevation-spine/refs/heads/main/security/elevation-spine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Health Care
- Spinal Implants
- Surgery
- Orthopedics
- Manufacturing
- Private Company
---
