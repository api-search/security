---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sensata.com
  spf: true
hosts:
- cert_expires: Oct  5 04:18:04 2026 GMT
  host: www.sensata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.sensata.com
  https: false
- host: api.sensata.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sensata Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensata Technologies, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sensata Technologies
provider_slug: sensata-technologies
slug: sensata-technologies-domain-security
source_filename: sensata-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sensata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:18:04 2026 GMT\n  hsts: null\n- host: developer.sensata.com\n  https: false\n- host: api.sensata.com\n  https: false\ndomains:\n- domain: sensata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensata-technologies/refs/heads/main/security/sensata-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sensors
- Electrical Protection
- Industrial
---
