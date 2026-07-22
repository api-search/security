---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: centreherbs.com
  spf: true
hosts:
- host: centreherbs.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''centreherbs'
kind: domain-security
layout: security
method: probed
name: Centreherbs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centreherbs (Beijing Shengtaier Biotechnology), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Centreherbs (Beijing Shengtaier Biotechnology)
provider_slug: centreherbs
slug: centreherbs-domain-security
source_filename: centreherbs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centreherbs.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''centreherbs'\n  hsts: null\ndomains:\n- domain: centreherbs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centreherbs/refs/heads/main/security/centreherbs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Veterinary
- Animal Health
- Traditional Chinese Medicine
- Pharmaceuticals
- Vaccines
- Feed Additives
- Biotechnology
- Healthcare
- China
---
