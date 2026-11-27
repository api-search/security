---
api_specs:
- filename: microsoft-365-copilot-connectors-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Connectors API
  slug: microsoft-365-copilot-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-connectors-api-openapi.yml
- filename: microsoft-365-copilot-external-items-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot External Items API
  slug: microsoft-365-copilot-external-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-external-items-api-openapi.yml
- filename: microsoft-365-copilot-search-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Search API
  slug: microsoft-365-copilot-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-search-api-openapi.yml
- filename: microsoft-365-copilot-user-content-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot User Content API
  slug: microsoft-365-copilot-user-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-user-content-api-openapi.yml
- filename: microsoft-365-copilot-copilot-aiinteractionhistory-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Copilot.ai Interaction History API
  slug: microsoft-365-copilot-copilot-aiinteractionhistory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-copilot-aiinteractionhistory-api-openapi.yml
- filename: microsoft-365-copilot-copilot-aiuser-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Copilot.ai User API
  slug: microsoft-365-copilot-copilot-aiuser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-copilot-aiuser-api-openapi.yml
- filename: microsoft-365-copilot-copilot-copilotadmin-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Copilot.copilot Admin API
  slug: microsoft-365-copilot-copilot-copilotadmin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-copilot-copilotadmin-api-openapi.yml
- filename: microsoft-365-copilot-copilot-copilotreportroot-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Copilot.copilot Report Root API
  slug: microsoft-365-copilot-copilot-copilotreportroot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-copilot-copilotreportroot-api-openapi.yml
- filename: microsoft-365-copilot-copilot-copilotroot-actions-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Copilot.copilot Root.Actions API
  slug: microsoft-365-copilot-copilot-copilotroot-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-copilot-copilotroot-actions-api-openapi.yml
- filename: microsoft-365-copilot-copilot-copilotroot-api-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot Copilot.copilot Root API
  slug: microsoft-365-copilot-copilot-copilotroot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-365-copilot/openapi/microsoft-365-copilot-copilot-copilotroot-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 18:34:59 2027 GMT
  host: api.powerplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft 365 Copilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft 365 Copilot, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft 365 Copilot
provider_slug: microsoft-365-copilot
slug: microsoft-365-copilot-domain-security
source_filename: microsoft-365-copilot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.powerplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:34:59 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-365-copilot/security/microsoft-365-copilot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Copilot
- Enterprise
- LLM
- Microsoft 365
- Natural Language Processing
- Productivity
---
