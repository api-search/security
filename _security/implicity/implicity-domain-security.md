---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: implicity.com
  spf: true
hosts:
- cert_expires: Sep 23 07:03:50 2026 GMT
  host: www.implicity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 06:08:39 2026 GMT
  host: implicity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: api.implicity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Implicity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Implicity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Implicity
provider_slug: implicity
slug: implicity-domain-security
source_filename: implicity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.implicity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:03:50 2026 GMT\n  hsts: false\n- host: implicity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 06:08:39 2026 GMT\n  hsts: false\n- host: api.implicity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: implicity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/implicity/refs/heads/main/security/implicity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health Tech
- Digital Health
- Remote Patient Monitoring
- Cardiology
- Medical Devices
- Cardiac Implantable Electronic Devices
- Artificial Intelligence
- EHR Integration
- Interoperability
- France
---
