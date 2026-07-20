---
api_specs:
- filename: impossible-cloud-management-console-openapi-original.json
  format: json
  label: Impossible Cloud Management Console API
  slug: impossible-cloud-management-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-cloud/refs/heads/main/openapi/impossible-cloud-management-console-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: impossiblecloud.com
  spf: true
hosts:
- cert_expires: Aug 31 09:22:57 2026 GMT
  host: www.impossiblecloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 09:03:39 2026 GMT
  host: docs.impossiblecloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 08:00:18 2026 GMT
  host: api.partner.impossiblecloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Impossible Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impossible Cloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Impossible Cloud
provider_slug: impossible-cloud
slug: impossible-cloud-domain-security
source_filename: impossible-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.impossiblecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:22:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.impossiblecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.partner.impossiblecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:00:18 2026 GMT\n  hsts: null\ndomains:\n- domain: impossiblecloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impossible-cloud/refs/heads/main/security/impossible-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Object Storage
- S3
- Storage
- Infrastructure
- GPU
- AI Infrastructure
- Data Sovereignty
- Europe
- GDPR
- Partner API
---
