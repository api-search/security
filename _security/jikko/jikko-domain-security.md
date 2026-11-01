---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jikko.com
  spf: true
hosts:
- host: jikko.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''jikko.com''.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jikko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jikko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Jikko
provider_slug: jikko
slug: jikko-domain-security
source_filename: jikko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jikko.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''jikko.com''.'\n  hsts: null\ndomains:\n- domain: jikko.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jikko/security/jikko-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
