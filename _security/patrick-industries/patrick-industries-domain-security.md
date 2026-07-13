---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: patrickind.com
  spf: true
hosts:
- cert_expires: Sep 10 17:58:08 2026 GMT
  host: www.patrickind.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.patrickind.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''developer.p'
- host: api.patrickind.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.patrick'
kind: domain-security
layout: security
method: probed
name: Patrick Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patrick Industries, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Patrick Industries
provider_slug: patrick-industries
slug: patrick-industries-domain-security
source_filename: patrick-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.patrickind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 17:58:08 2026 GMT\n  hsts: false\n- host: developer.patrickind.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''developer.p'\n  hsts: null\n- host: api.patrickind.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.patrick'\n  hsts: null\ndomains:\n- domain: patrickind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patrick-industries/refs/heads/main/security/patrick-industries-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Building Products
- RV
- Marine
---
