---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zilliz.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: zilliz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: docs.zilliz.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.cloud.zilliz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zilliz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zilliz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zilliz
provider_slug: zilliz
slug: zilliz-domain-security
source_filename: zilliz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zilliz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: docs.zilliz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n- host: api.cloud.zilliz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zilliz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zilliz/refs/heads/main/security/zilliz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vector Database
- AI
- Cloud
- Milvus
- Managed
---
