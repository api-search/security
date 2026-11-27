---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: org.ua
  spf: false
hosts:
- host: org.ua
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ORG.UA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ORG.UA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: ORG.UA
provider_slug: org-ua
slug: org-ua-domain-security
source_filename: org-ua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: org.ua\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: org.ua\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/org-ua/security/org-ua-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---
