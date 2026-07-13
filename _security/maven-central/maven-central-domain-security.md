---
api_specs:
- filename: maven-central-search-openapi.yml
  format: yaml
  label: Maven Central Search API
  slug: maven-central-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-central/refs/heads/main/openapi/maven-central-search-openapi.yml
- filename: maven-central-portal-openapi.yml
  format: yaml
  label: Central Portal Publishing API
  slug: central-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-central/refs/heads/main/openapi/maven-central-portal-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sonatype.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sonatype.org
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: central.sonatype.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: central.sonatype.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: search.maven.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maven Central Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maven Central, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Maven Central
provider_slug: maven-central
slug: maven-central-domain-security
source_filename: maven-central-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: central.sonatype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: false\n- host: central.sonatype.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: search.maven.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sonatype.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sonatype.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maven-central/refs/heads/main/security/maven-central-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artifacts
- Java
- JVM
- Maven
- Package Management
- Repository
---
