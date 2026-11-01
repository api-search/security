---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: propelo.ai
  spf: true
hosts:
- host: propelo.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Propelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propelo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Propelo
provider_slug: propelo
slug: propelo-domain-security
source_filename: propelo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: propelo.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: propelo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/propelo/security/propelo-domain-security.yml
summary_line: DMARC
tags:
- Company
---
