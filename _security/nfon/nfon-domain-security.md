---
api_specs:
- filename: nfon-pbx-configuration-api-openapi.json
  format: json
  label: NFON PBX Configuration API
  slug: nfon-pbx-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-pbx-configuration-api-openapi.json
- filename: nfon-cti-api-openapi.yml
  format: yaml
  label: NFON CTI API
  slug: nfon-cti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-cti-api-openapi.yml
- filename: nfon-call-history-api-openapi.yml
  format: yaml
  label: NFON Call History API
  slug: nfon-call-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-call-history-api-openapi.yml
- filename: nfon-service-portal-api.postman_collection.json
  format: json
  label: NFON Service Portal API (legacy)
  slug: nfon-service-portal-api-legacy
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/postman/nfon-service-portal-api.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nfon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nfon.net
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.nfon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.nfon.net
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: providersupportdata.cloud-cfg.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nfon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nfon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nfon
provider_slug: nfon
slug: nfon-domain-security
source_filename: nfon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nfon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nfon.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: providersupportdata.cloud-cfg.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nfon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nfon.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/security/nfon-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Telecom
- Cloud Telephony
- UCaaS
- CPaaS
- VoIP
- CTI
- Call History
- PBX
- Communications
- SIP
- Germany
---
