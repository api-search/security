---
api_specs:
- filename: optibus-operations-openapi.yml
  format: yaml
  label: Optibus Operations API
  slug: optibus-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optibus/refs/heads/main/openapi/optibus-operations-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: optibus.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: optibus.co
  spf: true
hosts:
- cert_expires: Sep 29 10:28:40 2026 GMT
  host: www.optibus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-optibus-account.api.ops.optibus.co
  https: false
kind: domain-security
layout: security
method: probed
name: Optibus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optibus, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Optibus
provider_slug: optibus
slug: optibus-domain-security
source_filename: optibus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optibus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:28:40 2026 GMT\n  hsts: false\n- host: your-optibus-account.api.ops.optibus.co\n  https: false\ndomains:\n- domain: optibus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: optibus.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optibus/refs/heads/main/security/optibus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Vertical Software
- Public Transportation
- Transit
- Scheduling
- Fleet Management
- Mobility
- Optimization
- Workforce Management
---
