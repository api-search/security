---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cardiovascular.abbott
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: st-jude-medical.com
  spf: false
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.cardiovascular.abbott
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: www.st-jude-medical.com
  https: false
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.abbott.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: St Jude Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for St. Jude Medical, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: St. Jude Medical
provider_slug: st-jude-medical
slug: st-jude-medical-domain-security
source_filename: st-jude-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cardiovascular.abbott\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.st-jude-medical.com\n  https: false\n- host: www.abbott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: cardiovascular.abbott\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: st-jude-medical.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/st-jude-medical/refs/heads/main/security/st-jude-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cardiac
- Cardiovascular
- Healthcare
- Medical Devices
- Patient Monitoring
- Remote Care
- Fortune 500
---
