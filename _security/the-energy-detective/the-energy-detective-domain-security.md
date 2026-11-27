---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: theenergydetective.com
  spf: true
hosts:
- host: theenergydetective.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''theenergyde'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TED (The Energy Detective) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TED (The Energy Detective), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TED (The Energy Detective)
provider_slug: the-energy-detective
slug: the-energy-detective-domain-security
source_filename: the-energy-detective-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theenergydetective.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''theenergyde'\n  hsts: null\ndomains:\n- domain: theenergydetective.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/the-energy-detective/security/the-energy-detective-domain-security.yml
summary_line: DMARC
tags:
- Company
- Energy
- Monitoring
- Home Automation
- IoT
---
