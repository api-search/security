---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trymonad.co
  spf: false
hosts:
- host: trymonad.co
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''trymonad.co'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trymonad Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Monad
provider_slug: trymonad-co
slug: trymonad-co-domain-security
source_filename: trymonad-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trymonad.co\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''trymonad.co'\n  hsts: null\ndomains:\n- domain: trymonad.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/trymonad-co/security/trymonad-co-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
