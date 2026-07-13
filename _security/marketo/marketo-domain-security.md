---
api_specs:
- filename: marketo-engage-rest-api-openapi.yml
  format: yaml
  label: Marketo Engage REST API
  slug: marketo-engage-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketo/refs/heads/main/openapi/marketo-engage-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marketo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
hosts:
- cert_expires: Aug 17 13:11:14 2026 GMT
  host: developers.marketo.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: experienceleague.adobe.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marketo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Marketo
provider_slug: marketo
slug: marketo-domain-security
source_filename: marketo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.marketo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 13:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: experienceleague.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: marketo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketo/refs/heads/main/security/marketo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Adobe
- Automation
- Marketing
- Marketing Automation
---
