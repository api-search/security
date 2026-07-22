---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vestahealthcare.com
  spf: true
hosts:
- host: www.vestahealthcare.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.vestahe'
kind: domain-security
layout: security
method: probed
name: Vesta Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vesta Healthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vesta Healthcare
provider_slug: vesta-healthcare
slug: vesta-healthcare-domain-security
source_filename: vesta-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vestahealthcare.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.vestahe'\n  hsts: null\ndomains:\n- domain: vestahealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vesta-healthcare/refs/heads/main/security/vesta-healthcare-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Healthcare
- Home Care
- Telehealth
- Caregivers
- Remote Patient Monitoring
- Chronic Care Management
- Medicare
- Value-Based Care
- Seniors
---
