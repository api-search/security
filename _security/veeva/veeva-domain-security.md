---
api_specs:
- filename: veeva-authentication-api-openapi.yml
  format: yaml
  label: veeva Authentication API
  slug: veeva-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-authentication-api-openapi.yml
- filename: veeva-documents-api-openapi.yml
  format: yaml
  label: veeva Documents API
  slug: veeva-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-documents-api-openapi.yml
- filename: veeva-objects-api-openapi.yml
  format: yaml
  label: veeva Objects API
  slug: veeva-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-objects-api-openapi.yml
- filename: veeva-query-api-openapi.yml
  format: yaml
  label: veeva Query API
  slug: veeva-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-query-api-openapi.yml
- filename: veeva-users-api-openapi.yml
  format: yaml
  label: veeva Users API
  slug: veeva-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-users-api-openapi.yml
- filename: veeva-workflows-api-openapi.yml
  format: yaml
  label: veeva Workflows API
  slug: veeva-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "starfieldtech.com"
  - 0 iodef "mailto:security-ops@veeva.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veeva.com
  spf: true
- caa:
  - 0 issuewild "thawte.com"
  - 0 iodef "mailto:security-ops@veeva.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veevavault.com
  spf: true
hosts:
- cert_expires: Oct 26 14:14:14 2026 GMT
  host: www.veeva.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: developer.veevavault.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: myvault.veevavault.com
  https: false
kind: domain-security
layout: security
method: probed
name: Veeva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for veeva, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: veeva
provider_slug: veeva
slug: veeva-domain-security
source_filename: veeva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veeva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 14:14:14 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.veevavault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\n- host: myvault.veevavault.com\n  https: false\ndomains:\n- domain: veeva.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 iodef \"mailto:security-ops@veeva.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: veevavault.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"thawte.com\"\n  - 0 iodef \"mailto:security-ops@veeva.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/security/veeva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Regulatory
- Quality Management
- Document-Management
- Content Management
- Healthcare
- Software-as-a-Service
- Enterprise
- MCP
- Agents
---
