---
api_specs:
- filename: keycloak-admin-rest-api-openapi.yml
  format: yaml
  label: Keycloak Admin REST API
  slug: admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-admin-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keycloak.org
  spf: true
hosts:
- cert_expires: Sep 18 02:17:21 2026 GMT
  host: www.keycloak.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keycloak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keycloak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Keycloak
provider_slug: keycloak
slug: keycloak-domain-security
source_filename: keycloak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keycloak.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:17:21 2026 GMT\n  hsts: false\ndomains:\n- domain: keycloak.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/security/keycloak-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Authentication
- Authorization
- Identity Management
- OAuth
- OpenID Connect
- Security
- SSO
---
