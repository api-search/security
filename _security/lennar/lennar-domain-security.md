---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lennar.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Sep 10 07:31:13 2026 GMT
  host: www.lennar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: azu-lndscapmu01e.portal.azure-api.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''azu-lndscap'
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: singlefamily.fanniemae.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lennar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lennar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lennar
provider_slug: lennar
slug: lennar-domain-security
source_filename: lennar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lennar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:31:13 2026 GMT\n  hsts: false\n- host: azu-lndscapmu01e.portal.azure-api.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''azu-lndscap'\n  hsts: null\n- host: singlefamily.fanniemae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lennar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lennar/refs/heads/main/security/lennar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Homebuilder
- Real Estate
- Fortune 500
- Mortgage
---
