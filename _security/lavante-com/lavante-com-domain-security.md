---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: lavante.com
  spf: true
hosts:
- host: www.lavante.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lavante Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lavante, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Lavante
provider_slug: lavante-com
slug: lavante-com-domain-security
source_filename: lavante-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lavante.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: lavante.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lavante-com/security/lavante-com-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Finance
- Analytics
- Procurement
- SaaS
---
