---
api_specs:
- filename: apache-jena-dataset-management-api-openapi.yml
  format: yaml
  label: Apache Jena Dataset Management API
  slug: apache-jena-dataset-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/openapi/apache-jena-dataset-management-api-openapi.yml
- filename: apache-jena-graph-store-protocol-api-openapi.yml
  format: yaml
  label: Apache Jena Graph Store Protocol API
  slug: apache-jena-graph-store-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/openapi/apache-jena-graph-store-protocol-api-openapi.yml
- filename: apache-jena-sparql-query-api-openapi.yml
  format: yaml
  label: Apache Jena SPARQL Query API
  slug: apache-jena-sparql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/openapi/apache-jena-sparql-query-api-openapi.yml
- filename: apache-jena-sparql-update-api-openapi.yml
  format: yaml
  label: Apache Jena SPARQL Update API
  slug: apache-jena-sparql-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/openapi/apache-jena-sparql-update-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: jena.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Jena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Jena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Jena
provider_slug: apache-jena
slug: apache-jena-domain-security
source_filename: apache-jena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jena.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/security/apache-jena-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
---
