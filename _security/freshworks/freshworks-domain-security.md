---
api_specs:
- filename: freshworks-freshdesk-api-openapi.yml
  format: yaml
  label: Freshworks Freshdesk API
  slug: freshdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshdesk-api-openapi.yml
- filename: freshworks-freshservice-api-openapi.yml
  format: yaml
  label: Freshworks Freshservice API
  slug: freshservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshservice-api-openapi.yml
- filename: freshworks-freshsales-api-openapi.yml
  format: yaml
  label: Freshworks Freshsales API
  slug: freshsales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshsales-api-openapi.yml
- filename: freshworks-freshchat-api-openapi.yml
  format: yaml
  label: Freshworks Freshchat API
  slug: freshchat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshchat-api-openapi.yml
- filename: freshworks-freshcaller-api-openapi.yml
  format: yaml
  label: Freshworks Freshcaller API
  slug: freshcaller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshcaller-api-openapi.yml
- filename: freshworks-freshteam-api-openapi.yml
  format: yaml
  label: Freshworks Freshteam API
  slug: freshteam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshteam-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freshdesk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freshservice.com
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: developers.freshdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: domain.freshdesk.com
  https: false
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.freshservice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for freshworks, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: freshworks
provider_slug: freshworks
slug: freshworks-domain-security
source_filename: freshworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: domain.freshdesk.com\n  https: false\n- host: api.freshservice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshdesk.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: freshservice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/security/freshworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
