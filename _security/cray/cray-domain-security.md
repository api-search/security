---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cray.com
  spf: true
hosts:
- host: cray.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''cray.com''. '
kind: domain-security
layout: security
method: probed
name: Cray Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cray, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cray
provider_slug: cray
slug: cray-domain-security
source_filename: cray-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cray.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''cray.com''. '\n  hsts: null\ndomains:\n- domain: cray.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cray/refs/heads/main/security/cray-domain-security.yml
summary_line: DMARC
tags:
- Company
- Supercomputing
- High Performance Computing
- HPC
- Hardware
- Data Center
- HPE
- Acquired
---
