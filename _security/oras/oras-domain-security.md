---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oras.land
  spf: false
hosts:
- cert_expires: Sep  1 02:37:11 2026 GMT
  host: oras.land
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oras Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ORAS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ORAS
provider_slug: oras
slug: oras-domain-security
source_filename: oras-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oras.land\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:37:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oras.land\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oras/refs/heads/main/security/oras-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artifact Storage
- Cloud Native
- Container Registry
- OCI
---
