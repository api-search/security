---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quakerhoughton.com
  spf: true
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.quakerhoughton.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.quakerhoughton.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''developer.q'
- host: api.quakerhoughton.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.quakerh'
kind: domain-security
layout: security
method: probed
name: Quaker Houghton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quaker Houghton, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quaker Houghton
provider_slug: quaker-houghton
slug: quaker-houghton-domain-security
source_filename: quaker-houghton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quakerhoughton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: false\n- host: developer.quakerhoughton.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''developer.q'\n  hsts: null\n- host: api.quakerhoughton.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.quakerh'\n  hsts: null\ndomains:\n- domain: quakerhoughton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/security/quaker-houghton-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial Fluids
- Chemical
- Manufacturing
---
