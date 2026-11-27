---
api_specs:
- filename: agentdatafeed-com-amsterdam-events-api-openapi.yml
  format: yaml
  label: AgentDataFeed Amsterdam Events API
  slug: agentdatafeed-com-amsterdam-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-amsterdam-events-api-openapi.yml
- filename: agentdatafeed-com-cert-advisories-api-openapi.yml
  format: yaml
  label: AgentDataFeed Cert Advisories API
  slug: agentdatafeed-com-cert-advisories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-cert-advisories-api-openapi.yml
- filename: agentdatafeed-com-datasets-api-openapi.yml
  format: yaml
  label: AgentDataFeed Datasets API
  slug: agentdatafeed-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-datasets-api-openapi.yml
- filename: agentdatafeed-com-drug-shortages-api-openapi.yml
  format: yaml
  label: AgentDataFeed Drug Shortages API
  slug: agentdatafeed-com-drug-shortages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-drug-shortages-api-openapi.yml
- filename: agentdatafeed-com-eu-funding-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Funding API
  slug: agentdatafeed-com-eu-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-funding-api-openapi.yml
- filename: agentdatafeed-com-eu-legislation-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Legislation API
  slug: agentdatafeed-com-eu-legislation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-legislation-api-openapi.yml
- filename: agentdatafeed-com-eu-medicines-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Medicines API
  slug: agentdatafeed-com-eu-medicines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-medicines-api-openapi.yml
- filename: agentdatafeed-com-eu-tenders-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Tenders API
  slug: agentdatafeed-com-eu-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-tenders-api-openapi.yml
- filename: agentdatafeed-com-feedback-api-openapi.yml
  format: yaml
  label: AgentDataFeed Feedback API
  slug: agentdatafeed-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-feedback-api-openapi.yml
- filename: agentdatafeed-com-product-recalls-api-openapi.yml
  format: yaml
  label: AgentDataFeed Product Recalls API
  slug: agentdatafeed-com-product-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-product-recalls-api-openapi.yml
- filename: agentdatafeed-com-public-holidays-api-openapi.yml
  format: yaml
  label: AgentDataFeed Public Holidays API
  slug: agentdatafeed-com-public-holidays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-public-holidays-api-openapi.yml
- filename: agentdatafeed-com-sanctions-entities-api-openapi.yml
  format: yaml
  label: AgentDataFeed Sanctions Entities API
  slug: agentdatafeed-com-sanctions-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-sanctions-entities-api-openapi.yml
- filename: agentdatafeed-com-security-advisories-api-openapi.yml
  format: yaml
  label: AgentDataFeed Security Advisories API
  slug: agentdatafeed-com-security-advisories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-security-advisories-api-openapi.yml
- filename: agentdatafeed-com-uk-tenders-api-openapi.yml
  format: yaml
  label: AgentDataFeed Uk Tenders API
  slug: agentdatafeed-com-uk-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-uk-tenders-api-openapi.yml
- filename: agentdatafeed-com-vulnerability-watch-api-openapi.yml
  format: yaml
  label: AgentDataFeed Vulnerability Watch API
  slug: agentdatafeed-com-vulnerability-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-vulnerability-watch-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@agentdatafeed.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: agentdatafeed.com
  spf: true
hosts:
- cert_expires: Jan  6 12:20:01 2027 GMT
  host: agentdatafeed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentDataFeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentDataFeed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AgentDataFeed
provider_slug: agentdatafeed-com
slug: agentdatafeed-com-domain-security
source_filename: agentdatafeed-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentdatafeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:20:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentdatafeed.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@agentdatafeed.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/agentdatafeed-com/security/agentdatafeed-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data
- Artificial Intelligence
- Public Sector
- Datasets
- Payments
---
