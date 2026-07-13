---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lhcgroup.com
  spf: true
hosts:
- cert_expires: Aug  5 14:28:01 2026 GMT
  host: www.lhcgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.lhcgroup.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''developer.l'
- host: api.lhcgroup.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.lhcgrou'
kind: domain-security
layout: security
method: probed
name: Lhc Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LHC Group, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LHC Group
provider_slug: lhc-group
slug: lhc-group-domain-security
source_filename: lhc-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lhcgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 14:28:01 2026 GMT\n  hsts: false\n- host: developer.lhcgroup.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''developer.l'\n  hsts: null\n- host: api.lhcgroup.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.lhcgrou'\n  hsts: null\ndomains:\n- domain: lhcgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lhc-group/refs/heads/main/security/lhc-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Home Health
- Hospice
- Healthcare
---
