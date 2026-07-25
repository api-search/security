---
api_specs:
- filename: lumos-accesspolicies-api-openapi.yml
  format: yaml
  label: Lumos AccessPolicies API
  slug: lumos-accesspolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accesspolicies-api-openapi.yml
- filename: lumos-accessrequests-api-openapi.yml
  format: yaml
  label: Lumos AccessRequests API
  slug: lumos-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessrequests-api-openapi.yml
- filename: lumos-accessreviews-api-openapi.yml
  format: yaml
  label: Lumos AccessReviews API
  slug: lumos-accessreviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessreviews-api-openapi.yml
- filename: lumos-accounts-api-openapi.yml
  format: yaml
  label: Lumos Accounts API
  slug: lumos-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accounts-api-openapi.yml
- filename: lumos-activity-api-openapi.yml
  format: yaml
  label: Lumos Activity API
  slug: lumos-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-activity-api-openapi.yml
- filename: lumos-apps-api-openapi.yml
  format: yaml
  label: Lumos Apps API
  slug: lumos-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-apps-api-openapi.yml
- filename: lumos-appstore-api-openapi.yml
  format: yaml
  label: Lumos AppStore API
  slug: lumos-appstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-appstore-api-openapi.yml
- filename: lumos-groups-api-openapi.yml
  format: yaml
  label: Lumos Groups API
  slug: lumos-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-groups-api-openapi.yml
- filename: lumos-preapprovalrules-api-openapi.yml
  format: yaml
  label: Lumos PreApprovalRules API
  slug: lumos-preapprovalrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-preapprovalrules-api-openapi.yml
- filename: lumos-tasks-api-openapi.yml
  format: yaml
  label: Lumos Tasks API
  slug: lumos-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-tasks-api-openapi.yml
- filename: lumos-users-api-openapi.yml
  format: yaml
  label: Lumos Users API
  slug: lumos-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-users-api-openapi.yml
- filename: lumos-utility-api-openapi.yml
  format: yaml
  label: Lumos Utility API
  slug: lumos-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-utility-api-openapi.yml
- filename: lumos-vendors-api-openapi.yml
  format: yaml
  label: Lumos Vendors API
  slug: lumos-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-vendors-api-openapi.yml
- filename: lumos-webhooks-api-openapi.yml
  format: yaml
  label: Lumos Webhooks API
  slug: lumos-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lumos.com
  spf: true
hosts:
- cert_expires: Sep 11 20:44:01 2026 GMT
  host: www.lumos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 19:52:28 2026 GMT
  host: developers.lumos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: api.lumos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lumos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lumos
provider_slug: lumos
slug: lumos-domain-security
source_filename: lumos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lumos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:44:01 2026 GMT\n  hsts: false\n- host: developers.lumos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:52:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lumos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lumos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/security/lumos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Management
- Access Reviews
- Deprovisioning
- Identity Governance
- Identity Platform
- Least Privilege
- Provisioning
- SaaS Management
- Shadow IT
---
