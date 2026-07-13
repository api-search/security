---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dtic.mil
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: dodtechspace.mil
  spf: false
hosts:
- host: www.dtic.mil
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: discover.dtic.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.dodtechspace.mil
  https: false
kind: domain-security
layout: security
method: probed
name: Defense Technical Information Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Technical Information Center, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Technical Information Center
provider_slug: defense-technical-information-center
slug: defense-technical-information-center-domain-security
source_filename: defense-technical-information-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dtic.mil\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: discover.dtic.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.dodtechspace.mil\n  https: false\ndomains:\n- domain: dtic.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dodtechspace.mil\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-technical-information-center/refs/heads/main/security/defense-technical-information-center-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Defense
- Department of Defense
- DTIC
- Federal Government
- Knowledge Management
- Library
- Research
- Scientific and Technical Information
---
