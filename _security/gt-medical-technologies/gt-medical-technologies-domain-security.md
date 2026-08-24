---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gammatile.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: gammatile.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gt Medical Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GT Medical Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GT Medical Technologies
provider_slug: gt-medical-technologies
slug: gt-medical-technologies-domain-security
source_filename: gt-medical-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gammatile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gammatile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gt-medical-technologies/refs/heads/main/security/gt-medical-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Oncology
- Radiation Therapy
- Brachytherapy
- Neurosurgery
- Brain Tumors
- Medical Technology
- Arizona
---
