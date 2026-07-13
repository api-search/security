---
api_specs:
- filename: yardi-voyager-api-openapi.yml
  format: yaml
  label: Yardi Voyager API
  slug: yardi-voyager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi/refs/heads/main/openapi/yardi-voyager-api-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yardi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rentcafe.com
  spf: true
hosts:
- cert_expires: Oct  6 02:36:40 2026 GMT
  host: www.yardi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.yardi.com
  https: false
- cert_expires: Sep 20 08:00:16 2026 GMT
  host: www.rentcafe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yardi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yardi, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yardi
provider_slug: yardi
slug: yardi-domain-security
source_filename: yardi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yardi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.yardi.com\n  https: false\n- host: www.rentcafe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:00:16 2026 GMT\n  hsts: false\ndomains:\n- domain: yardi.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rentcafe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi/refs/heads/main/security/yardi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Commercial Real Estate
- Coworking
- Investment Management
- Multifamily
- Property Management
- Real Estate
- Residential
- Self Storage
- Senior Living
---
