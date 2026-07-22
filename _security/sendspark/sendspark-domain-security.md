---
api_specs:
- filename: sendspark-openapi-original.json
  format: json
  label: Sendspark API
  slug: sendspark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sendspark.com
  spf: true
hosts:
- cert_expires: Sep 15 19:11:06 2026 GMT
  host: sendspark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:47:54 2026 GMT
  host: api-gw.sendspark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sendspark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sendspark, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sendspark
provider_slug: sendspark
slug: sendspark-domain-security
source_filename: sendspark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendspark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:11:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-gw.sendspark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:47:54 2026 GMT\n  hsts: null\ndomains:\n- domain: sendspark.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/security/sendspark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Sales
- Marketing
- Personalization
- Artificial Intelligence
- Video Messaging
- Webhooks
- MCP
---
