---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uitgis.com
  spf: true
hosts:
- host: uitgis.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''uitgis.com'''
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jungdo Uit Co Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JUNGDO UIT CO., LTD., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: JUNGDO UIT CO., LTD.
provider_slug: jungdo-uit-co-ltd
slug: jungdo-uit-co-ltd-domain-security
source_filename: jungdo-uit-co-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uitgis.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''uitgis.com'''\n  hsts: null\ndomains:\n- domain: uitgis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jungdo-uit-co-ltd/security/jungdo-uit-co-ltd-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- GIS
- Mapping
- Urban Planning
- Government Solutions
---
