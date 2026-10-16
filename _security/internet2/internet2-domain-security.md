---
api_specs:
- filename: internet2-co-api-openapi.yml
  format: yaml
  label: Internet2 Co API
  slug: internet2-co-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-api-openapi.yml
- filename: internet2-co-group-members-api-openapi.yml
  format: yaml
  label: Internet2 Co Group Members API
  slug: internet2-co-group-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-group-members-api-openapi.yml
- filename: internet2-co-group-members-json-api-openapi.yml
  format: yaml
  label: Internet2 Co Group Members.json API
  slug: internet2-co-group-members-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-group-members-json-api-openapi.yml
- filename: internet2-co-groups-api-openapi.yml
  format: yaml
  label: Internet2 Co Groups API
  slug: internet2-co-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-groups-api-openapi.yml
- filename: internet2-co-groups-json-api-openapi.yml
  format: yaml
  label: Internet2 Co Groups.json API
  slug: internet2-co-groups-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-groups-json-api-openapi.yml
- filename: internet2-co-people-api-openapi.yml
  format: yaml
  label: Internet2 Co People API
  slug: internet2-co-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-people-api-openapi.yml
- filename: internet2-co-people-json-api-openapi.yml
  format: yaml
  label: Internet2 Co People.json API
  slug: internet2-co-people-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-people-json-api-openapi.yml
- filename: internet2-email-addresses-json-api-openapi.yml
  format: yaml
  label: Internet2 Email Addresses.json API
  slug: internet2-email-addresses-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-email-addresses-json-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: internet2.edu
  spf: true
hosts:
- cert_expires: Apr  4 14:32:16 2027 GMT
  host: internet2.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Internet2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internet2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Internet2
provider_slug: internet2
slug: internet2-domain-security
source_filename: internet2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: internet2.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 14:32:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: internet2.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/security/internet2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Networking
- Research
- Education
- Nonprofit
---
