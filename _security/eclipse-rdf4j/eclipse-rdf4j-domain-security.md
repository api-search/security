---
api_specs:
- filename: rdf4j-server-rest-api-openapi.yml
  format: yaml
  label: RDF4J Server REST API
  slug: rdf4j-server-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse-rdf4j/main/openapi/rdf4j-server-rest-api-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: rdf4j.org
  spf: false
hosts:
- cert_expires: Aug 15 14:54:51 2026 GMT
  host: rdf4j.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eclipse Rdf4J Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eclipse RDF4J, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Eclipse RDF4J
provider_slug: eclipse-rdf4j
slug: eclipse-rdf4j-domain-security
source_filename: eclipse-rdf4j-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rdf4j.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 14:54:51 2026 GMT\n  hsts: false\ndomains:\n- domain: rdf4j.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eclipse-rdf4j/refs/heads/main/security/eclipse-rdf4j-domain-security.yml
summary_line: TLSv1.3
tags:
- Eclipse Foundation
- Java
- Linked Data
- Open Source
- RDF
- Semantic Web
- SPARQL
- Triple Store
---
