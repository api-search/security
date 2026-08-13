---
api_specs:
- filename: workfront-planning-v2-openapi.json
  format: json
  label: Adobe Workfront Planning API v2
  slug: workfront-planning-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/openapi/workfront-planning-v2-openapi.json
- filename: workfront-planning-v1-openapi.json
  format: json
  label: Adobe Workfront Planning API v1
  slug: workfront-planning-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/openapi/workfront-planning-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: workfront.com
  note: legacy Workfront domain; www.workfront.com no longer resolves (NXDOMAIN) since the move to business.adobe.com, but the apex retains SPF and a DMARC reject policy
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: business.adobe.com
  hsts: null
  https: true
  note: unreachable over HTTP/2 from the probing network (curl 92 INTERNAL_ERROR); TLS handshake and certificate validated
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: experienceleague.adobe.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: mcp.workfront.adobe.com
  hsts: false
  https: true
  note: MCP server host; root path returns 404, the MCP endpoint is /mcp/v1/workfront
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api-cl01.my.workfront.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: public reference instance backing the API Explorer; serves the anonymous object-metadata contract
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: developersupport.workfront.com
  hsts: false
  https: true
  note: hosts the Workfront API Explorer application
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workfront Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Workfront, probed live across 6 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Workfront
provider_slug: workfront
slug: workfront-domain-security
source_filename: workfront-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: The three hosts below the divider were added by hand because the apis.yml baseURLs for the core\n  and Planning APIs are per-customer templated hosts, so the mechanical probe could not reach them. The\n  reference/API-Explorer instance (api-cl01.my.workfront.com), the MCP host and the developer-support\n  host are the real, reachable equivalents.\nhosts:\n- host: business.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n  note: unreachable over HTTP/2 from the probing network (curl 92 INTERNAL_ERROR); TLS handshake and\n    certificate validated\n- host: experienceleague.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts:\
  \ true\n  hsts_max_age: 31557600\n- host: mcp.workfront.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: false\n  note: MCP server host; root path returns 404, the MCP endpoint is /mcp/v1/workfront\n- host: api-cl01.my.workfront.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: public reference instance backing the API Explorer; serves the anonymous object-metadata contract\n- host: developersupport.workfront.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n  note: hosts the Workfront API Explorer application\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: workfront.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: reject\n  note: legacy\
  \ Workfront domain; www.workfront.com no longer resolves (NXDOMAIN) since the move to\n    business.adobe.com, but the apex retains SPF and a DMARC reject policy\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/security/workfront-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Work Management
- Project Management
- Marketing Operations
- Creative Operations
- Collaboration
- Approvals
- Resource Management
- Workflow Automation
- Enterprise Software
- Adobe
- Model Context Protocol
---
