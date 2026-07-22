---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datasci.com
  spf: true
hosts:
- cert_expires: Sep 11 02:34:46 2026 GMT
  host: www.datasci.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Sciences International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Sciences International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Data Sciences International
provider_slug: data-sciences-international
slug: data-sciences-international-domain-security
source_filename: data-sciences-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datasci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:34:46 2026 GMT\n  hsts: false\ndomains:\n- domain: datasci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-sciences-international/refs/heads/main/security/data-sciences-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Preclinical Research
- Physiology
- Telemetry
- Medical Devices
- Laboratory Instruments
- Data Analysis
---
