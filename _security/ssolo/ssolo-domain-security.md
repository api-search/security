---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ssolo.eu
  spf: true
hosts:
- host: ssolo.eu
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''ssolo.eu''. '
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ssolo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SSOLO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SSOLO
provider_slug: ssolo
slug: ssolo-domain-security
source_filename: ssolo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ssolo.eu\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''ssolo.eu''. '\n  hsts: null\ndomains:\n- domain: ssolo.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ssolo/security/ssolo-domain-security.yml
summary_line: DMARC
tags:
- Company
- SSO
- Identity
- Authentication
- Security
---
