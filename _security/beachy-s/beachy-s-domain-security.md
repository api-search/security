---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: beachy.com
  spf: true
hosts:
- host: www.beachy.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.beachy.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beachy S Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beachy''s, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Beachy's
provider_slug: beachy-s
slug: beachy-s-domain-security
source_filename: beachy-s-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beachy.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.beachy.'\n  hsts: null\ndomains:\n- domain: beachy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beachy-s/refs/heads/main/security/beachy-s-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Email
- RealNames
- Domain
- Personalization
- Tucows
---
