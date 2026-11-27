---
api_specs:
- filename: keeperhub-com-chains-api-openapi.yml
  format: yaml
  label: KeeperHub Chains API
  slug: keeperhub-com-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-chains-api-openapi.yml
- filename: keeperhub-com-health-api-openapi.yml
  format: yaml
  label: KeeperHub Health API
  slug: keeperhub-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-health-api-openapi.yml
- filename: keeperhub-com-keys-api-openapi.yml
  format: yaml
  label: KeeperHub Keys API
  slug: keeperhub-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-keys-api-openapi.yml
- filename: keeperhub-com-mcp-api-openapi.yml
  format: yaml
  label: KeeperHub MCP API
  slug: keeperhub-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-mcp-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@keeperhub.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: keeperhub.com
  spf: true
hosts:
- cert_expires: Feb  5 10:29:28 2027 GMT
  host: keeperhub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KeeperHub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeeperHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KeeperHub
provider_slug: keeperhub-com
slug: keeperhub-com-domain-security
source_filename: keeperhub-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keeperhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 10:29:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keeperhub.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@keeperhub.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/keeperhub-com/security/keeperhub-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Artificial Intelligence
- Automation
- DeFi
- Onchain
- Company
---
