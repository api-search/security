---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: motorolasolutions.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rapiddeploy.com
  spf: true
hosts:
- cert_expires: Oct 27 18:18:08 2026 GMT
  host: www.motorolasolutions.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 18:19:33 2026 GMT
  host: api.rapiddeploy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapiddeploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RapidDeploy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RapidDeploy
provider_slug: rapiddeploy
slug: rapiddeploy-domain-security
source_filename: rapiddeploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.motorolasolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 18:18:08 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.rapiddeploy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:19:33 2026 GMT\n  hsts: null\ndomains:\n- domain: motorolasolutions.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rapiddeploy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapiddeploy/refs/heads/main/security/rapiddeploy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Public Safety
- Emergency Services
- NG911
- Computer-Aided Dispatch
- Mapping
- Analytics
- Government
- Cloud
---
