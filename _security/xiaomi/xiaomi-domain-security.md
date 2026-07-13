---
api_specs:
- filename: xiaomi-open-api-openapi.yml
  format: yaml
  label: Xiaomi Open API
  slug: xiaomi-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-open-api-openapi.yml
- filename: xiaomi-galaxy-fds-openapi.yml
  format: yaml
  label: Xiaomi Galaxy FDS API
  slug: xiaomi-galaxy-fds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-galaxy-fds-openapi.yml
- filename: xiaomi-mimo-api-openapi.yml
  format: yaml
  label: Xiaomi MiMo AI API
  slug: xiaomi-mimo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-mimo-api-openapi.yml
description: ''
domains:
- caa:
  - sgp.ali.cdn.b2cop.lb.mi.com.
  dmarc: false
  dnssec: true
  domain: mi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xiaomi.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.mi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: dev.mi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 16 01:53:07 2026 GMT
  host: open.account.xiaomi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xiaomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xiaomi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Xiaomi
provider_slug: xiaomi
slug: xiaomi-domain-security
source_filename: xiaomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\n- host: dev.mi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\n- host: open.account.xiaomi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 16 01:53:07 2026 GMT\n  hsts: null\ndomains:\n- domain: mi.com\n  dnssec: true\n  caa:\n  - sgp.ali.cdn.b2cop.lb.mi.com.\n  spf: true\n  dmarc: false\n- domain: xiaomi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/security/xiaomi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Consumer Electronics
- IoT
- Smart Home
- Mobile
- Artificial Intelligence
- Cloud Storage
- Machine Learning
---
