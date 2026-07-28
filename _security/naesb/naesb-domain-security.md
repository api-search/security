---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: naesb.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oati.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.naesb.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: www.naesbwry.oati.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Naesb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NAESB, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NAESB
provider_slug: naesb
slug: naesb-domain-security
source_filename: naesb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.naesb.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\n- host: www.naesbwry.oati.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: naesb.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: oati.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naesb/refs/heads/main/security/naesb-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Energy
- United States
- Standards
- Utilities
- Electricity
- Gas
- Green Button
- Smart Metering
- Energy Markets
- Grid
---
