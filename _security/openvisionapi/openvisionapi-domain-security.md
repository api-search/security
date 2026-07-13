---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openvisionapi.com
  spf: false
hosts:
- host: openvisionapi.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Openvisionapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenVisionAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenVisionAPI
provider_slug: openvisionapi
slug: openvisionapi-domain-security
source_filename: openvisionapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openvisionapi.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: openvisionapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openvisionapi/refs/heads/main/security/openvisionapi-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Machine Learning
- Public APIs
---
