---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: contactually.com
  spf: false
hosts:
- host: contactually.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Contactually Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contactually, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Contactually
provider_slug: contactually
slug: contactually-domain-security
source_filename: contactually-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contactually.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: contactually.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contactually/refs/heads/main/security/contactually-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- CRM
- Customer Relationship Management
- Real Estate
- Contact Management
- Relationships
- Sales
- Defunct
---
