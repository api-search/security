---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ilook.fit
  spf: true
hosts:
- cert_expires: Dec 28 14:44:08 2026 GMT
  host: www.ilook.fit
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ilook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iLook AI Face Analysis (Wallic Technologies), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: iLook AI Face Analysis (Wallic Technologies)
provider_slug: ilook
slug: ilook-domain-security
source_filename: ilook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ilook.fit\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 14:44:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ilook.fit\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ilook/refs/heads/main/security/ilook-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- FaceAnalysis
- ImageProcessing
- Biometrics
---
