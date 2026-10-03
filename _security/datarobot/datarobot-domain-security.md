---
api_specs:
- filename: datarobot-openapi-generated.yml
  format: yaml
  label: DataRobot API
  slug: datarobot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarobot/refs/heads/main/openapi/_ae-authored/datarobot-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datarobot.com
  spf: true
hosts:
- cert_expires: Dec 25 12:09:31 2026 GMT
  host: datarobot.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: docs.datarobot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: app.datarobot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Datarobot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataRobot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataRobot
provider_slug: datarobot
slug: datarobot-domain-security
source_filename: datarobot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datarobot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 12:09:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: docs.datarobot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.datarobot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datarobot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datarobot/refs/heads/main/security/datarobot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- MLOps
- Data Science
- Agentic AI
- Predictive Analytics
- Generative AI
---
