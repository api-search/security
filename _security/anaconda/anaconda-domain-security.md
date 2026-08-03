---
api_specs:
- filename: anaconda-server-openapi-original.json
  format: json
  label: Anaconda Server API
  slug: server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-server-openapi-original.json
- filename: anaconda-org-management-openapi-original.json
  format: json
  label: Anaconda Organization Management API
  slug: org-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-org-management-openapi-original.json
- filename: anaconda-audit-logs-openapi-original.json
  format: json
  label: Anaconda Audit Logs API
  slug: audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-audit-logs-openapi-original.json
- filename: anaconda-ai-navigator-openapi-original.json
  format: json
  label: Anaconda AI Navigator API
  slug: ai-navigator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-ai-navigator-openapi-original.json
- filename: anaconda-desktop-openapi-original.json
  format: json
  label: Anaconda Desktop API
  slug: desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-desktop-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anaconda.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anaconda.cloud
  spf: true
hosts:
- cert_expires: Sep  3 06:20:54 2026 GMT
  host: www.anaconda.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 01:15:08 2026 GMT
  host: anaconda.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 22:04:51 2026 GMT
  host: api.anaconda.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anaconda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anaconda, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anaconda
provider_slug: anaconda
slug: anaconda-domain-security
source_filename: anaconda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anaconda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:20:54 2026 GMT\n  hsts: false\n- host: anaconda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:15:08 2026 GMT\n  hsts: false\n- host: api.anaconda.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:04:51 2026 GMT\n  hsts: null\ndomains:\n- domain: anaconda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: anaconda.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/security/anaconda-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Data Science
- Machine Learning
- Artificial Intelligence
- Package Management
- Python
- Developer Tools
- Software Supply Chain
- Repository
- Package Registry
- Conda
- MCP
---
