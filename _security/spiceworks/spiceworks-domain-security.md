---
api_specs:
- filename: spiceworks-cloud-apps-openapi.yml
  format: yaml
  label: Spiceworks Cloud Apps API
  slug: spiceworks-cloud-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiceworks/refs/heads/main/openapi/spiceworks-cloud-apps-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:dns@spiceworks.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spiceworks.com
  spf: true
hosts:
- cert_expires: Aug 30 01:44:12 2026 GMT
  host: community.spiceworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spiceworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spiceworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spiceworks
provider_slug: spiceworks
slug: spiceworks-domain-security
source_filename: spiceworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.spiceworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:44:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spiceworks.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:dns@spiceworks.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiceworks/refs/heads/main/security/spiceworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Community
- Enterprise IT
- IT Management
---
