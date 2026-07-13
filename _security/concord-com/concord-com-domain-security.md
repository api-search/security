---
api_specs:
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Agreements API
  slug: concord-com-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Organizations & Users API
  slug: concord-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Documents & Attachments API
  slug: concord-com-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Templates API
  slug: concord-com-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: concordnow.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:email.chargebee.com include:26737077.spf03.hubspotemail.net -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: concord.app
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:email.chargebee.com include:26737077.spf03.hubspotemail.net -all
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M01
  cert_subject: CN=concordnow.com
  host: api.concordnow.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Live REST API host. GET /api/rest/1/user/me returns HTTP 401 {"statusCode":401,"restCode":"unauthorized"} without a valid X-API-KEY.
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  cert_issuer: ZeroSSL ECC DV SSL CA 2
  cert_subject: CN=www.concord.app
  host: www.concord.app
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  note: Marketing site, served via Framer (sites.framer.app).
  tls_version: TLSv1.3
- cert_issuer: Let's Encrypt
  host: concord.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Redirects to https://www.concord.app/.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Concord Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Concord, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Concord
provider_slug: concord-com
slug: concord-com-domain-security
source_filename: concord-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API hosts\nhosts:\n- host: api.concordnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=concordnow.com\n  cert_issuer: Amazon RSA 2048 M01\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Live REST API host. GET /api/rest/1/user/me returns HTTP 401 {\"statusCode\":401,\"restCode\":\"unauthorized\"} without a valid X-API-KEY.\n- host: www.concord.app\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=www.concord.app\n  cert_issuer: ZeroSSL ECC DV SSL CA 2\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  note: Marketing site, served via Framer (sites.framer.app).\n- host: concord.app\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  hsts: true\n  hsts_max_age: 31536000\n  note: Redirects to https://www.concord.app/.\n\
  domains:\n- domain: concordnow.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:email.chargebee.com include:26737077.spf03.hubspotemail.net -all'\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: concord.app\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:email.chargebee.com include:26737077.spf03.hubspotemail.net -all'\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/security/concord-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- Agreements
- E-Signature
- Document Management
- Legal
- Workflow
---
