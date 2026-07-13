---
api_specs:
- filename: sonatype-nexus-repository-openapi.yml
  format: yaml
  label: Nexus Repository API
  slug: nexus-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonatype-nexus/refs/heads/main/openapi/sonatype-nexus-repository-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sonatype.com
  spf: true
hosts:
- cert_expires: Sep 10 18:41:02 2026 GMT
  host: www.sonatype.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:31:57 2026 GMT
  host: help.sonatype.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonatype Nexus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonatype Nexus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sonatype Nexus
provider_slug: sonatype-nexus
slug: sonatype-nexus-domain-security
source_filename: sonatype-nexus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonatype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:41:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.sonatype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:31:57 2026 GMT\n  hsts: false\ndomains:\n- domain: sonatype.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonatype-nexus/refs/heads/main/security/sonatype-nexus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artifact Management
- DevOps
- Package Management
- Repository
- Maven
- npm
- Docker
- Software Supply Chain
---
