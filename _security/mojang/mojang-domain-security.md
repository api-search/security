---
api_specs:
- filename: mojang-public-api-openapi.yml
  format: yaml
  label: Mojang Public API
  slug: mojang-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-public-api-openapi.yml
- filename: mojang-session-server-openapi.yml
  format: yaml
  label: Mojang Session Server
  slug: mojang-session-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-session-server-openapi.yml
- filename: mojang-minecraft-services-openapi.yml
  format: yaml
  label: Minecraft Services API
  slug: minecraft-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-minecraft-services-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "microsoft.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: minecraft.net
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: minecraft.wiki
  spf: true
hosts:
- cert_expires: Jan 22 16:56:36 2027 GMT
  host: www.minecraft.net
  hsts: true
  hsts_max_age: 7884000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:01:15 2026 GMT
  host: minecraft.wiki
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 22:44:42 2026 GMT
  host: api.mojang.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mojang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mojang, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mojang
provider_slug: mojang
slug: mojang-domain-security
source_filename: mojang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.minecraft.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 16:56:36 2027 GMT\n  hsts: true\n  hsts_max_age: 7884000\n- host: minecraft.wiki\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:01:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mojang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 22:44:42 2026 GMT\n  hsts: null\ndomains:\n- domain: minecraft.net\n  dnssec: false\n  caa:\n  - 0 issue \"microsoft.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: minecraft.wiki\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/security/mojang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Games And Comics
- Minecraft
- Gaming
- Identity
- Player Profiles
- Session
- Public APIs
---
