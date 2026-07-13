---
api_specs:
- filename: dokploy-openapi.yml
  format: yaml
  label: Dokploy
  slug: dokploy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dokploy/refs/heads/main/openapi/dokploy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dokploy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-dokploy-instance.com
  spf: false
hosts:
- cert_expires: Sep 21 21:30:18 2026 GMT
  host: dokploy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-dokploy-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Dokploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dokploy, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dokploy
provider_slug: dokploy
slug: dokploy-domain-security
source_filename: dokploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dokploy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:30:18 2026 GMT\n  hsts: false\n- host: your-dokploy-instance.com\n  https: false\ndomains:\n- domain: dokploy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: your-dokploy-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dokploy/refs/heads/main/security/dokploy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- PaaS
- Self-Hosted
- Open Source
- Docker
- Docker Swarm
- Deployment
- Traefik
- Databases
---
