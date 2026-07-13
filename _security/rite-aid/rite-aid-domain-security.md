---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rite-aid.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: riteaidediservices.com
  spf: false
hosts:
- host: www.rite-aid.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: www.riteaidediservices.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.riteaid'
- cert_expires: Aug 26 17:49:06 2026 GMT
  host: riteaid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rite Aid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rite Aid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rite Aid
provider_slug: rite-aid
slug: rite-aid-domain-security
source_filename: rite-aid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rite-aid.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: www.riteaidediservices.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.riteaid'\n  hsts: null\n- host: riteaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:49:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rite-aid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: riteaidediservices.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rite-aid/refs/heads/main/security/rite-aid-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- EDI
- Fortune 500
- Health
- Pharmacy
- Prescriptions
- Retail
---
