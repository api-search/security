---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unidesk.com
  spf: true
hosts:
- host: www.unidesk.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.unidesk'
kind: domain-security
layout: security
method: probed
name: Unidesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unidesk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unidesk
provider_slug: unidesk
slug: unidesk-domain-security
source_filename: unidesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unidesk.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.unidesk'\n  hsts: null\ndomains:\n- domain: unidesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unidesk/refs/heads/main/security/unidesk-domain-security.yml
summary_line: DMARC
tags:
- Company
- Infrastructure
- Virtualization
- Desktop Virtualization
- Application Layering
- VDI
- Acquired
---
