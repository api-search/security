---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kikolabs.com
  spf: true
hosts:
- host: kikolabs.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''kikolabs.co'
kind: domain-security
layout: security
method: probed
name: Kiko Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiko Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kiko Labs
provider_slug: kiko-labs
slug: kiko-labs-domain-security
source_filename: kiko-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kikolabs.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''kikolabs.co'\n  hsts: null\ndomains:\n- domain: kikolabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiko-labs/refs/heads/main/security/kiko-labs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Education
- EdTech
- Children
- Neuroscience
- Cognitive Training
- Mobile App
- Executive Function
---
