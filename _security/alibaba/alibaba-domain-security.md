---
api_specs:
- filename: alibaba-openapi.yml
  format: yaml
  label: Alibaba Cloud API
  slug: alibaba-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alibaba/refs/heads/main/openapi/alibaba-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alibaba.com
  spf: true
- caa:
  - 0 iodef "mailto:certificate-transparency@list.alibaba-inc.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alibabacloud.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.alibaba.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 02:26:16 2026 GMT
  host: www.alibabacloud.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  5 02:26:16 2026 GMT
  host: api.alibabacloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alibaba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alibaba, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alibaba
provider_slug: alibaba
slug: alibaba-domain-security
source_filename: alibaba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alibaba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.alibabacloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 02:26:16 2026 GMT\n  hsts: null\n- host: api.alibabacloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:26:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alibaba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: alibabacloud.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:certificate-transparency@list.alibaba-inc.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alibaba/refs/heads/main/security/alibaba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Cloud Computing
- E-Commerce
- Commerce
- AI
- Machine Learning
- Big Data
- Storage
- Networking
- Serverless
- Developer Tools
---
