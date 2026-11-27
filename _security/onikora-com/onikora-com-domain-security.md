---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onikora.com
  spf: true
hosts:
- host: onikora.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1147)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: onikora-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for onikora-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: onikora-com
provider_slug: onikora-com
slug: onikora-com-domain-security
source_filename: onikora-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onikora.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1147)'\n  hsts: null\ndomains:\n- domain: onikora.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/onikora-com/security/onikora-com-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
