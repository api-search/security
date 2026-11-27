---
api_specs:
- filename: justidea-agency-agents-api-openapi.yml
  format: yaml
  label: JustIdea Agents API
  slug: justidea-agency-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-agents-api-openapi.yml
- filename: justidea-agency-contact-api-openapi.yml
  format: yaml
  label: JustIdea Contact API
  slug: justidea-agency-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-contact-api-openapi.yml
- filename: justidea-agency-content-api-openapi.yml
  format: yaml
  label: JustIdea Content API
  slug: justidea-agency-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-content-api-openapi.yml
- filename: justidea-agency-meta-api-openapi.yml
  format: yaml
  label: JustIdea Meta API
  slug: justidea-agency-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-meta-api-openapi.yml
- filename: justidea-agency-offer-api-openapi.yml
  format: yaml
  label: JustIdea Offer API
  slug: justidea-agency-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-offer-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: justidea.agency
  spf: true
hosts:
- cert_expires: Feb  5 11:20:18 2027 GMT
  host: justidea.agency
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JustIdea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JustIdea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: JustIdea
provider_slug: justidea-agency
slug: justidea-agency-domain-security
source_filename: justidea-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justidea.agency\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 11:20:18 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: justidea.agency\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/justidea-agency/security/justidea-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- Agency
- Poland
- PrestaShop
- WooCommerce
---
