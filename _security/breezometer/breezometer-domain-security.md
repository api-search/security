---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: breezometer.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: mapsplatform.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 18:13:18 2026 GMT
  host: docs.breezometer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 18:11:39 2026 GMT
  host: api.breezometer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breezometer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BreezoMeter, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BreezoMeter
provider_slug: breezometer
slug: breezometer-domain-security
source_filename: breezometer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapsplatform.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: false\n- host: docs.breezometer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:13:18 2026 GMT\n  hsts: false\n- host: api.breezometer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:11:39 2026 GMT\n  hsts: false\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: breezometer.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breezometer/refs/heads/main/security/breezometer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Air Quality
- Environment
- Pollen
- Wildfire
- Weather
- Environmental Intelligence
---
