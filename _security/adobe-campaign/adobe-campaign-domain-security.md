---
api_specs:
- filename: adobe-campaign-standard-openapi-original.yml
  format: yaml
  label: Adobe Campaign Standard API
  slug: standard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-standard-openapi-original.yml
- filename: adobe-campaign-classic-openapi-original.yml
  format: yaml
  label: Adobe Campaign Classic API
  slug: classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-classic-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: experienceleague.adobe.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:48:09 2026 GMT
  host: opensource.adobe.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Adobe Campaign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Campaign, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Campaign
provider_slug: adobe-campaign
slug: adobe-campaign-domain-security
source_filename: adobe-campaign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: experienceleague.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: opensource.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 20 22:48:09 2026 GMT\n  hsts: false\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/security/adobe-campaign-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
---
