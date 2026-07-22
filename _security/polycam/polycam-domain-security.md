---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: poly.cam
  spf: true
hosts:
- cert_expires: Aug 26 05:12:42 2026 GMT
  host: poly.cam
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polycam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polycam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Polycam
provider_slug: polycam
slug: polycam-domain-security
source_filename: polycam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poly.cam\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: poly.cam\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polycam/refs/heads/main/security/polycam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- 3D Scanning
- 3D Capture
- Photogrammetry
- LiDAR
- Gaussian Splatting
- NeRF
- Floor Plans
- Drone Mapping
- Spatial Computing
- Mobile Capture
- AEC
- VFX
- Mesh Export
- glTF
- USDZ
---
