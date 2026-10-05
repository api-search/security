---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brainsgate.com
  spf: true
hosts:
- host: www.brainsgate.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.brainsg'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainsgate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrainsGate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BrainsGate
provider_slug: brainsgate
slug: brainsgate-domain-security
source_filename: brainsgate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brainsgate.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.brainsg'\n  hsts: null\ndomains:\n- domain: brainsgate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainsgate/refs/heads/main/security/brainsgate-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Medical Devices
- Neurotechnology
- CNS Therapy
- Israel
- Innovation
---
