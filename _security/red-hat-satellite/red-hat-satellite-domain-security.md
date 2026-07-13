---
api_specs:
- filename: v2.json
  format: json
  label: Red Hat Satellite REST API
  slug: red-hat-satellite-rest-api
  spec_type: OpenAPI
  url: https://satellite.example.com/apidoc/v2.json
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
  dmarc: false
  dnssec: false
  domain: theforeman.org
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: access.redhat.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: docs.redhat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 07:00:20 2027 GMT
  host: theforeman.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Red Hat Satellite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Hat Satellite, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
slug: red-hat-satellite-domain-security
source_filename: red-hat-satellite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: access.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: docs.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: theforeman.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 07:00:20 2027 GMT\n  hsts: false\ndomains:\n- domain: redhat.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:it-cert-admin@redhat.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: theforeman.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/security/red-hat-satellite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
---
