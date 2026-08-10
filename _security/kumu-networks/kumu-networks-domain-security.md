---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kumunetworks.com
  spf: true
hosts:
- host: kumunetworks.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''kumunetwork'
kind: domain-security
layout: security
method: probed
name: Kumu Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kumu Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kumu Networks
provider_slug: kumu-networks
slug: kumu-networks-domain-security
source_filename: kumu-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kumunetworks.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''kumunetwork'\n  hsts: null\ndomains:\n- domain: kumunetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kumu-networks/refs/heads/main/security/kumu-networks-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Semiconductors
- Wireless
- RF
- Spectrum
- Full Duplex
- 5G
- Telecommunications
- Defense
- IoT
- Hardware
---
