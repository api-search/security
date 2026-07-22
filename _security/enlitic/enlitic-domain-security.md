---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: enlitic.com
  spf: true
hosts:
- cert_expires: Sep 27 02:10:56 2026 GMT
  host: enlitic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enlitic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enlitic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Enlitic
provider_slug: enlitic
slug: enlitic-domain-security
source_filename: enlitic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enlitic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:10:56 2026 GMT\n  hsts: false\ndomains:\n- domain: enlitic.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enlitic/refs/heads/main/security/enlitic-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Digital Biology
- Healthcare
- Medical Imaging
- Radiology
- Artificial Intelligence
- DICOM
- Data Standardization
- Anonymization
---
