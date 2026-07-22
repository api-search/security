---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: foundationmedicine.com
  spf: true
hosts:
- cert_expires: Oct 16 06:25:43 2026 GMT
  host: foundationmedicine.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Foundation Medicine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foundation Medicine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Foundation Medicine
provider_slug: foundation-medicine
slug: foundation-medicine-domain-security
source_filename: foundation-medicine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foundationmedicine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:25:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: foundationmedicine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foundation-medicine/refs/heads/main/security/foundation-medicine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Genomics
- Cancer Diagnostics
- Precision Medicine
- Molecular Profiling
- Healthcare
---
