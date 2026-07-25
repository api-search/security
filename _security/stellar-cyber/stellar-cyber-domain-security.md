---
api_specs:
- filename: stellar-cyber-alerts-api-openapi.yml
  format: yaml
  label: Stellar Cyber Alerts API
  slug: stellar-cyber-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-alerts-api-openapi.yml
- filename: stellar-cyber-authentication-api-openapi.yml
  format: yaml
  label: Stellar Cyber Authentication API
  slug: stellar-cyber-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-authentication-api-openapi.yml
- filename: stellar-cyber-cases-api-openapi.yml
  format: yaml
  label: Stellar Cyber Cases API
  slug: stellar-cyber-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-cases-api-openapi.yml
- filename: stellar-cyber-connectors-api-openapi.yml
  format: yaml
  label: Stellar Cyber Connectors API
  slug: stellar-cyber-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-connectors-api-openapi.yml
- filename: stellar-cyber-events-api-openapi.yml
  format: yaml
  label: Stellar Cyber Events API
  slug: stellar-cyber-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-events-api-openapi.yml
- filename: stellar-cyber-playbooks-api-openapi.yml
  format: yaml
  label: Stellar Cyber Playbooks API
  slug: stellar-cyber-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-playbooks-api-openapi.yml
- filename: stellar-cyber-queries-api-openapi.yml
  format: yaml
  label: Stellar Cyber Queries API
  slug: stellar-cyber-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-queries-api-openapi.yml
- filename: stellar-cyber-reports-api-openapi.yml
  format: yaml
  label: Stellar Cyber Reports API
  slug: stellar-cyber-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-reports-api-openapi.yml
- filename: stellar-cyber-sensors-api-openapi.yml
  format: yaml
  label: Stellar Cyber Sensors API
  slug: stellar-cyber-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-sensors-api-openapi.yml
- filename: stellar-cyber-tenants-api-openapi.yml
  format: yaml
  label: Stellar Cyber Tenants API
  slug: stellar-cyber-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-tenants-api-openapi.yml
- filename: stellar-cyber-watchlists-api-openapi.yml
  format: yaml
  label: Stellar Cyber Watchlists API
  slug: stellar-cyber-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/openapi/stellar-cyber-watchlists-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stellarcyber.ai
  spf: true
hosts:
- cert_expires: Nov 23 15:49:09 2026 GMT
  host: stellarcyber.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 15:49:09 2026 GMT
  host: docs.stellarcyber.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stellar Cyber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stellar Cyber, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Stellar Cyber
provider_slug: stellar-cyber
slug: stellar-cyber-domain-security
source_filename: stellar-cyber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stellarcyber.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 15:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.stellarcyber.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 15:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: stellarcyber.ai\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellar-cyber/refs/heads/main/security/stellar-cyber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- Security
- XDR
- SIEM
- SOAR
- AI
---
