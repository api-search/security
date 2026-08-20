---
api_specs:
- filename: curse-categories-api-openapi.yml
  format: yaml
  label: Curse Categories API
  slug: curse-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-categories-api-openapi.yml
- filename: curse-files-api-openapi.yml
  format: yaml
  label: Curse Files API
  slug: curse-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-files-api-openapi.yml
- filename: curse-fingerprints-api-openapi.yml
  format: yaml
  label: Curse Fingerprints API
  slug: curse-fingerprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-fingerprints-api-openapi.yml
- filename: curse-games-api-openapi.yml
  format: yaml
  label: Curse Games API
  slug: curse-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-games-api-openapi.yml
- filename: curse-minecraft-api-openapi.yml
  format: yaml
  label: Curse Minecraft API
  slug: curse-minecraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-minecraft-api-openapi.yml
- filename: curse-mods-api-openapi.yml
  format: yaml
  label: Curse Mods API
  slug: curse-mods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-mods-api-openapi.yml
- filename: curse-subscriptions-api-openapi.yml
  format: yaml
  label: Curse Subscriptions API
  slug: curse-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/openapi/curse-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:domains@fandom.com"
  - 0 iodef "mailto:ops-l@fandom.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fandom.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: curseforge.com
  spf: true
hosts:
- cert_expires: Oct 13 12:56:52 2026 GMT
  host: www.fandom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.curseforge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curse, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curse
provider_slug: curse
slug: curse-domain-security
source_filename: curse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fandom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 12:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.curseforge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fandom.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:domains@fandom.com\"\n  - 0 iodef \"mailto:ops-l@fandom.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: curseforge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curse/refs/heads/main/security/curse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- MODS
- Minecraft
- Game Content
- Developer Platform
- Catalog
---
