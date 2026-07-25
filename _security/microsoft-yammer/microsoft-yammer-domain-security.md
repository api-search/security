---
api_specs:
- filename: microsoft-yammer-files-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Files API
  slug: microsoft-yammer-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-files-api-openapi.yml
- filename: microsoft-yammer-groups-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Groups API
  slug: microsoft-yammer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-groups-api-openapi.yml
- filename: microsoft-yammer-messages-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Messages API
  slug: microsoft-yammer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-messages-api-openapi.yml
- filename: microsoft-yammer-networks-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Networks API
  slug: microsoft-yammer-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-networks-api-openapi.yml
- filename: microsoft-yammer-search-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Search API
  slug: microsoft-yammer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-search-api-openapi.yml
- filename: microsoft-yammer-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Subscriptions API
  slug: microsoft-yammer-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-subscriptions-api-openapi.yml
- filename: microsoft-yammer-threads-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Threads API
  slug: microsoft-yammer-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-threads-api-openapi.yml
- filename: microsoft-yammer-topics-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Topics API
  slug: microsoft-yammer-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-topics-api-openapi.yml
- filename: microsoft-yammer-users-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Users API
  slug: microsoft-yammer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 issue "microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cloud.microsoft
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 29 18:44:29 2026 GMT
  host: engage.cloud.microsoft
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 18:44:29 2026 GMT
  host: www.yammer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Yammer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Yammer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Yammer
provider_slug: microsoft-yammer
slug: microsoft-yammer-domain-security
source_filename: microsoft-yammer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engage.cloud.microsoft\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 18:44:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.yammer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 18:44:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloud.microsoft\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 issue \"microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/security/microsoft-yammer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Enterprise Social
- Microsoft
- Social Networking
- Viva Engage
- Yammer
---
