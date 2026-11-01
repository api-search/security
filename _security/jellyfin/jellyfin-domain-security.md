---
api_specs:
- filename: jellyfin-openapi-generated.yml
  format: yaml
  label: Jellyfin API
  slug: jellyfin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jellyfin/openapi/_ae-authored/jellyfin-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jellyfin.org
  spf: true
hosts:
- cert_expires: Dec 29 03:49:51 2026 GMT
  host: jellyfin.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jellyfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jellyfin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jellyfin
provider_slug: jellyfin
slug: jellyfin-domain-security
source_filename: jellyfin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jellyfin.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 03:49:51 2026 GMT\n  hsts: false\ndomains:\n- domain: jellyfin.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jellyfin/security/jellyfin-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Media
- Open-Source
- Free-Software
- Community
- Streaming
- Company
---
