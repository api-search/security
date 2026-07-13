---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stepan.com
  spf: true
hosts:
- host: www.stepan.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: developer.stepan.com
  https: false
- host: api.stepan.com
  https: false
kind: domain-security
layout: security
method: probed
name: Stepan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stepan Company, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stepan Company
provider_slug: stepan
slug: stepan-domain-security
source_filename: stepan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stepan.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: developer.stepan.com\n  https: false\n- host: api.stepan.com\n  https: false\ndomains:\n- domain: stepan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stepan/refs/heads/main/security/stepan-domain-security.yml
summary_line: DMARC
tags:
- Specialty Chemicals
- Surfactants
---
