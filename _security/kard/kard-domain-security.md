---
api_specs:
- filename: kard-attributions-api-openapi.yml
  format: yaml
  label: Kard attributions API
  slug: kard-attributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-attributions-api-openapi.yml
- filename: kard-files-api-openapi.yml
  format: yaml
  label: Kard Files API
  slug: kard-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-files-api-openapi.yml
- filename: kard-notifications-notifications-api-openapi.yml
  format: yaml
  label: Kard notifications > Notifications API
  slug: kard-notifications-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-notifications-notifications-api-openapi.yml
- filename: kard-notifications-subscriptions-api-openapi.yml
  format: yaml
  label: Kard notifications > Subscriptions API
  slug: kard-notifications-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-notifications-subscriptions-api-openapi.yml
- filename: kard-organizations-api-openapi.yml
  format: yaml
  label: Kard Organizations API
  slug: kard-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-api-openapi.yml
- filename: kard-organizations-children-api-openapi.yml
  format: yaml
  label: Kard Organizations > Children API
  slug: kard-organizations-children-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-children-api-openapi.yml
- filename: kard-organizations-contentstrategies-api-openapi.yml
  format: yaml
  label: Kard Organizations > ContentStrategies API
  slug: kard-organizations-contentstrategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-contentstrategies-api-openapi.yml
- filename: kard-organizations-placements-api-openapi.yml
  format: yaml
  label: Kard Organizations > Placements API
  slug: kard-organizations-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-placements-api-openapi.yml
- filename: kard-ping-api-openapi.yml
  format: yaml
  label: Kard Ping API
  slug: kard-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-ping-api-openapi.yml
- filename: kard-rewards-api-openapi.yml
  format: yaml
  label: Kard rewards API
  slug: kard-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-rewards-api-openapi.yml
- filename: kard-transactions-api-openapi.yml
  format: yaml
  label: Kard transactions API
  slug: kard-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-transactions-api-openapi.yml
- filename: kard-users-api-openapi.yml
  format: yaml
  label: Kard users API
  slug: kard-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-api-openapi.yml
- filename: kard-users-attributions-api-openapi.yml
  format: yaml
  label: Kard users > attributions API
  slug: kard-users-attributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-attributions-api-openapi.yml
- filename: kard-users-rewards-api-openapi.yml
  format: yaml
  label: Kard users > Rewards API
  slug: kard-users-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-rewards-api-openapi.yml
- filename: kard-users-uploads-api-openapi.yml
  format: yaml
  label: Kard users > uploads API
  slug: kard-users-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-uploads-api-openapi.yml
- filename: kard-users-webview-api-openapi.yml
  format: yaml
  label: Kard users > WebView API
  slug: kard-users-webview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-webview-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getkard.com
  spf: true
hosts:
- cert_expires: Aug 24 20:29:31 2026 GMT
  host: getkard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kard
provider_slug: kard
slug: kard-domain-security
source_filename: kard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getkard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:29:31 2026 GMT\n  hsts: null\ndomains:\n- domain: getkard.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/security/kard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Rewards
- Card-Linked Offers
- Loyalty
- Fintech
- Commerce Media
- Advertising
- Transaction
- Cashback
- Webhook
---
