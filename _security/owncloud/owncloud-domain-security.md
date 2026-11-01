---
api_specs:
- filename: owncloud-openapi-generated.yml
  format: yaml
  label: ownCloud API
  slug: owncloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/owncloud/openapi/_ae-authored/owncloud-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: owncloud.com
  spf: true
hosts:
- cert_expires: Jan 24 16:32:14 2027 GMT
  host: owncloud.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Owncloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ownCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ownCloud
provider_slug: owncloud
slug: owncloud-domain-security
source_filename: owncloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: owncloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 16:32:14 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: owncloud.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/owncloud/security/owncloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Sharing
- Secure Collaboration
- Cloud Storage
- Data Sovereignty
- SaaS
- On-Premises
- Compliance
---
