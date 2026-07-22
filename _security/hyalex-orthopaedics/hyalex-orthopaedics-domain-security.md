---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyalex.com
  spf: true
hosts:
- cert_expires: Oct 11 08:27:06 2026 GMT
  host: hyalex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyalex Orthopaedics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyalex Orthopaedics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hyalex Orthopaedics
provider_slug: hyalex-orthopaedics
slug: hyalex-orthopaedics-domain-security
source_filename: hyalex-orthopaedics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyalex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 08:27:06 2026 GMT\n  hsts: false\ndomains:\n- domain: hyalex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyalex-orthopaedics/refs/heads/main/security/hyalex-orthopaedics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Orthopedics
- MedTech
- Health
- Biotechnology
- Implants
---
