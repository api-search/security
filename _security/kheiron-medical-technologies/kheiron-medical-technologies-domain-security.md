---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kheironmed.com
  spf: true
hosts:
- cert_expires: Sep 17 05:42:09 2026 GMT
  host: www.kheironmed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kheiron Medical Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kheiron Medical Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kheiron Medical Technologies
provider_slug: kheiron-medical-technologies
slug: kheiron-medical-technologies-domain-security
source_filename: kheiron-medical-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kheironmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:42:09 2026 GMT\n  hsts: false\ndomains:\n- domain: kheironmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kheiron-medical-technologies/refs/heads/main/security/kheiron-medical-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Medical Imaging
- Artificial Intelligence
- Radiology
- Breast Cancer Screening
- Diagnostics
---
