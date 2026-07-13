---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dbpedia.org
  spf: false
hosts:
- cert_expires: Oct  3 12:04:40 2026 GMT
  host: www.dbpedia.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 01:05:38 2026 GMT
  host: dbpedia.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 08:11:57 2026 GMT
  host: lookup.dbpedia.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dbpedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DBpedia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DBpedia
provider_slug: dbpedia
slug: dbpedia-domain-security
source_filename: dbpedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dbpedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:04:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: dbpedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:05:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: lookup.dbpedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 08:11:57 2026 GMT\n  hsts: false\ndomains:\n- domain: dbpedia.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbpedia/refs/heads/main/security/dbpedia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Linked Data
- Knowledge Graph
- SPARQL
- Semantic Web
- Wikipedia
- Open Data
- Entity Linking
- RDF
- Ontology
---
