---
api_specs:
- filename: swagger.v3.json
  format: json
  label: Confluence Cloud REST API v1
  slug: confluence-cloud-rest-api-v1
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/confluence/swagger.v3.json
- filename: openapi.yaml
  format: yaml
  label: Confluence Cloud REST API v2
  slug: confluence-cloud-rest-api-v2
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/confluence/rest/v2/api-spec/
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atlassian.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: your-domain.atlassian.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confluence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confluence, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Confluence
provider_slug: confluence
slug: confluence-domain-security
source_filename: confluence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-domain.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atlassian.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\
  \n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/security/confluence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
---
