---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wxqa.com
  spf: false
hosts:
- host: www.wxqa.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cwop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citizen Weather Observer Program, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Citizen Weather Observer Program
provider_slug: cwop
slug: cwop-domain-security
source_filename: cwop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wxqa.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: wxqa.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cwop/security/cwop-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Weather
- CitizenScience
- DataCollection
- PublicPrivatePartnership
- Community
---
