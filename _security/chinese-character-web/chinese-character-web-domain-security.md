---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hemiola.com
  spf: true
hosts:
- host: ccdb.hemiola.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''ccdb.hemiol'
kind: domain-security
layout: security
method: probed
name: Chinese Character Web Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chinese Character Web, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chinese Character Web
provider_slug: chinese-character-web
slug: chinese-character-web-domain-security
source_filename: chinese-character-web-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ccdb.hemiola.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''ccdb.hemiol'\n  hsts: null\ndomains:\n- domain: hemiola.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chinese-character-web/refs/heads/main/security/chinese-character-web-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Dictionaries
- Public APIs
---
