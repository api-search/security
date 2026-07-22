---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pinnaclefoods.com
  spf: true
hosts:
- host: www.pinnaclefoods.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.pinnacl'
kind: domain-security
layout: security
method: probed
name: Pinnacle Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pinnacle-foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: pinnacle-foods
provider_slug: pinnacle-foods
slug: pinnacle-foods-domain-security
source_filename: pinnacle-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinnaclefoods.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.pinnacl'\n  hsts: null\ndomains:\n- domain: pinnaclefoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle-foods/refs/heads/main/security/pinnacle-foods-domain-security.yml
summary_line: DMARC
tags:
- Fortune 1000
---
