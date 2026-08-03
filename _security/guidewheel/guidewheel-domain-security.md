---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: guidewheel.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: guidewheel.app
  spf: true
hosts:
- cert_expires: Oct 12 12:26:48 2026 GMT
  host: www.guidewheel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 14:48:04 2026 GMT
  host: support.guidewheel.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 14:48:04 2026 GMT
  host: app.guidewheel.app
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guidewheel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guidewheel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Guidewheel
provider_slug: guidewheel
slug: guidewheel-domain-security
source_filename: guidewheel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guidewheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:26:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.guidewheel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 14:48:04 2026 GMT\n  hsts: false\n- host: app.guidewheel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 14:48:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: guidewheel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: guidewheel.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewheel/refs/heads/main/security/guidewheel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Industrial IoT
- Machine Monitoring
- OEE
- FactoryOps
- Predictive Maintenance
- Energy
- Sensors
- Telemetry
---
