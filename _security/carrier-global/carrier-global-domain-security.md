---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carrier.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: carrier.io
  spf: true
hosts:
- cert_expires: Aug 30 04:21:23 2026 GMT
  host: www.corporate.carrier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:43:45 2026 GMT
  host: api.tta.lynxfleet.carrier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: doc-api.fleet.lynx.carrier.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carrier Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carrier Global, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carrier Global
provider_slug: carrier-global
slug: carrier-global-domain-security
source_filename: carrier-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corporate.carrier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 04:21:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tta.lynxfleet.carrier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc-api.fleet.lynx.carrier.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: carrier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: carrier.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrier-global/refs/heads/main/security/carrier-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HVAC
- Cold Chain
- Telematics
- Building Automation
- IoT
- Refrigeration
- Fortune 500
---
