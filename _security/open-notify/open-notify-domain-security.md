---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: open-notify.org
  spf: false
hosts:
- host: open-notify.org
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''open-notify'
kind: domain-security
layout: security
method: probed
name: Open Notify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Notify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Notify
provider_slug: open-notify
slug: open-notify-domain-security
source_filename: open-notify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-notify.org\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''open-notify'\n  hsts: null\ndomains:\n- domain: open-notify.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-notify/refs/heads/main/security/open-notify-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Science And Math
- Public APIs
---
