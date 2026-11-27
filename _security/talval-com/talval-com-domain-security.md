---
api_specs:
- filename: talval-com-agent-api-openapi.yml
  format: yaml
  label: Talval Agent API
  slug: talval-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talval-com/openapi/talval-com-agent-api-openapi.yml
- filename: talval-com-daily-api-openapi.yml
  format: yaml
  label: Talval Daily API
  slug: talval-com-daily-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talval-com/openapi/talval-com-daily-api-openapi.yml
- filename: talval-com-learn-feed-api-openapi.yml
  format: yaml
  label: Talval Learn Feed API
  slug: talval-com-learn-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talval-com/openapi/talval-com-learn-feed-api-openapi.yml
- filename: talval-com-superinvestors-api-openapi.yml
  format: yaml
  label: Talval Superinvestors API
  slug: talval-com-superinvestors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talval-com/openapi/talval-com-superinvestors-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    agents: []
    checked: '2026-11-26'
    index:
    - alpn:
      - h2
      target: talval.com
    published: true
  dnssec: true
  domain: talval.com
  spf: true
hosts:
- cert_expires: Feb 10 15:19:18 2027 GMT
  host: talval.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Talval Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talval, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Talval
provider_slug: talval-com
slug: talval-com-domain-security
source_filename: talval-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talval.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 15:19:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: talval.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: true\n    index:\n    - target: talval.com\n      alpn:\n      - h2\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/talval-com/security/talval-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Stock Research
- Value Investing
- Financial Data
- Analytics
---
