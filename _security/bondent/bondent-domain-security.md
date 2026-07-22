---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bondent.com
  spf: true
hosts:
- cert_expires: Jul 23 23:59:59 2026 GMT
  host: bondent.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bondent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bondent (博恩登特), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bondent (博恩登特)
provider_slug: bondent
slug: bondent-domain-security
source_filename: bondent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bondent.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bondent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bondent/refs/heads/main/security/bondent-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Dental
- Oral Healthcare
- Medical Devices
- Dental Imaging
- CBCT
- Digital Dentistry
- Clinic Management
- Healthcare
- China
---
