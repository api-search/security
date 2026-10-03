---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boshihitech.com
  spf: true
hosts:
- host: boshihitech.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''boshihitech'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boshihitech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boshihitech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Boshihitech
provider_slug: boshihitech
slug: boshihitech-domain-security
source_filename: boshihitech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boshihitech.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''boshihitech'\n  hsts: null\ndomains:\n- domain: boshihitech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boshihitech/refs/heads/main/security/boshihitech-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Technology
- Automation
- IoT
- Manufacturing
---
