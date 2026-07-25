---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pensando.io
  spf: true
hosts:
- host: pensando.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''pensando.io'
kind: domain-security
layout: security
method: probed
name: Pensando Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pensando *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pensando *
provider_slug: pensando
slug: pensando-domain-security
source_filename: pensando-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pensando.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''pensando.io'\n  hsts: null\ndomains:\n- domain: pensando.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pensando/refs/heads/main/security/pensando-domain-security.yml
summary_line: DMARC
tags:
- Company
- Enterprise
- Networking
- DPU
- Infrastructure
- Cloud
- Security
- AMD
---
