---
api_specs:
- filename: mimecast-com-openapi-generated.yml
  format: yaml
  label: ProjectDiscovery API
  slug: mimecast-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mimecast-com/openapi/_ae-authored/mimecast-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "pki.goog"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mimecast.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: protect-eu.mimecast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mimecast Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProjectDiscovery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ProjectDiscovery
provider_slug: mimecast-com
slug: mimecast-com-domain-security
source_filename: mimecast-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: protect-eu.mimecast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mimecast.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mimecast-com/security/mimecast-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vulnerability Management
- Offensive Security
- Cloud Security
- Open Source Tools
---
