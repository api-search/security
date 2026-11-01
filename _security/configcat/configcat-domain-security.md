---
api_specs:
- filename: configcat-openapi.json
  format: json
  label: ConfigCat Public Management API
  slug: configcat-public-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configcat/openapi/configcat-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: configcat.com
  spf: true
hosts:
- cert_expires: Jan 15 00:41:06 2027 GMT
  host: configcat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Configcat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConfigCat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ConfigCat
provider_slug: configcat
slug: configcat-domain-security
source_filename: configcat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: configcat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 00:41:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: configcat.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/configcat/security/configcat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Feature-Flag
- SaaS
- Developer-Tools
- API
- Cloud
---
