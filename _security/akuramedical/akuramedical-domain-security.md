---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: akuramedical.com
  spf: false
hosts:
- cert_expires: Dec 11 12:54:47 2026 GMT
  host: www.akuramedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Akuramedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akura Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Akura Medical
provider_slug: akuramedical
slug: akuramedical-domain-security
source_filename: akuramedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akuramedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 12:54:47 2026 GMT\n  hsts: false\ndomains:\n- domain: akuramedical.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akuramedical/refs/heads/main/security/akuramedical-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- MedicalDevice
- VascularHealth
- Thrombectomy
- Innovation
---
