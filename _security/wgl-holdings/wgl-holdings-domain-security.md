---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wglholdings.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: washingtongas.com
  spf: true
hosts:
- cert_expires: Aug  2 20:27:37 2026 GMT
  host: www.wglholdings.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 03:00:22 2026 GMT
  host: www.washingtongas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: www.wglenergy.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Wgl Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WGL Holdings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WGL Holdings
provider_slug: wgl-holdings
slug: wgl-holdings-domain-security
source_filename: wgl-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wglholdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 20:27:37 2026 GMT\n  hsts: null\n- host: www.washingtongas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 03:00:22 2026 GMT\n  hsts: false\n- host: www.wglenergy.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: wglholdings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: washingtongas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wgl-holdings/refs/heads/main/security/wgl-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Natural Gas
- Utilities
- Electricity
- Retail Energy
- Midstream
- Fortune 1000
---
