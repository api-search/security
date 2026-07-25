---
api_specs:
- filename: microsoft-linkedin-adaccounts-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdAccounts API
  slug: microsoft-linkedin-adaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adaccounts-api-openapi.yml
- filename: microsoft-linkedin-adaccountusers-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdAccountUsers API
  slug: microsoft-linkedin-adaccountusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adaccountusers-api-openapi.yml
- filename: microsoft-linkedin-adcampaigngroups-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdCampaignGroups API
  slug: microsoft-linkedin-adcampaigngroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adcampaigngroups-api-openapi.yml
- filename: microsoft-linkedin-adcampaigns-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdCampaigns API
  slug: microsoft-linkedin-adcampaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adcampaigns-api-openapi.yml
- filename: microsoft-linkedin-adcreatives-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdCreatives API
  slug: microsoft-linkedin-adcreatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adcreatives-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Linkedin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft LinkedIn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft LinkedIn
provider_slug: microsoft-linkedin
slug: microsoft-linkedin-domain-security
source_filename: microsoft-linkedin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/security/microsoft-linkedin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Microsoft
- Professional Networking
- Recruiting
- Social Network
---
