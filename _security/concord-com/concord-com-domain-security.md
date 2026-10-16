---
api_specs:
- filename: concord-com-agreements-api-openapi.yml
  format: yaml
  label: Concord Agreements API
  slug: concord-com-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-agreements-api-openapi.yml
- filename: concord-com-organizations-api-openapi.yml
  format: yaml
  label: Concord Organizations API
  slug: concord-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-organizations-api-openapi.yml
- filename: concord-com-templates-api-openapi.yml
  format: yaml
  label: Concord Templates API
  slug: concord-com-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-templates-api-openapi.yml
- filename: concord-com-users-api-openapi.yml
  format: yaml
  label: Concord Users API
  slug: concord-com-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: concord.app
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: concordnow.com
  spf: true
hosts:
- cert_expires: Nov 21 15:01:51 2026 GMT
  host: www.concord.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 22:42:05 2026 GMT
  host: help.concord.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: api.concordnow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Concord Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Concord, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Concord
provider_slug: concord-com
slug: concord-com-domain-security
source_filename: concord-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.concord.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 15:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.concord.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 22:42:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.concordnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: concord.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: concordnow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/security/concord-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Contract Management
- Contract Lifecycle Management
- Contracts
- Agreements
- E-Signature
- Document Management
- Legal
- Workflows
---
