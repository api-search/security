---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ablativesolutions.com
  spf: true
hosts:
- host: ablativesolutions.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ablative Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ablative Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ablative Solutions
provider_slug: ablative-solutions
slug: ablative-solutions-domain-security
source_filename: ablative-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ablativesolutions.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ablativesolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ablative-solutions/refs/heads/main/security/ablative-solutions-domain-security.yml
summary_line: DMARC
tags:
- Company
- Medical Devices
- Health
- Hypertension
- Renal Denervation
- Cardiovascular
- Clinical Research
- Life Sciences
---
