---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imagen.ai
  spf: true
hosts:
- cert_expires: Aug 31 06:05:06 2026 GMT
  host: imagen.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imagen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imagen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Imagen
provider_slug: imagen
slug: imagen-domain-security
source_filename: imagen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imagen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:05:06 2026 GMT\n  hsts: false\ndomains:\n- domain: imagen.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imagen/refs/heads/main/security/imagen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Frontier Tech
- Healthcare
- Radiology
- Medical Imaging
- Teleradiology
- Artificial Intelligence
- Diagnostics
---
