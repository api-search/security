---
api_specs:
- filename: OpenAPI.yaml
  format: yaml
  label: JBoss EAP Management API
  slug: jboss-eap-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/wildfly/wildfly/main/docs/src/main/asciidoc/_admin-guide/management-api/OpenAPI.yaml
- filename: openapi.json
  format: json
  label: Keycloak Admin REST API
  slug: keycloak-admin-rest-api
  spec_type: OpenAPI
  url: https://www.keycloak.org/docs-api/latest/rest-api/openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:it-cert-admin@redhat.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redhat.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wildfly.org
  spf: false
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: developers.redhat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: access.redhat.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 12:10:21 2026 GMT
  host: wildfly.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jboss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JBoss, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JBoss
provider_slug: jboss
slug: jboss-domain-security
source_filename: jboss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\n- host: access.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: wildfly.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:10:21 2026 GMT\n  hsts: false\ndomains:\n- domain: redhat.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:it-cert-admin@redhat.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wildfly.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jboss/refs/heads/main/security/jboss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Server
- Cloud Native
- Enterprise
- Jakarta EE
- Java EE
- Microservices
- Middleware
- Open Source
- Red Hat
---
