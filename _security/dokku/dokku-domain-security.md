---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dokku.com
  spf: false
hosts:
- cert_expires: Sep  6 05:25:37 2026 GMT
  host: dokku.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dokku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dokku, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dokku
provider_slug: dokku
slug: dokku-domain-security
source_filename: dokku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dokku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:25:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: dokku.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dokku/refs/heads/main/security/dokku-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- PaaS
- Self-Hosted
- Docker
- Containers
- Buildpacks
- Deployment
- DevOps
- Heroku Alternative
- Open Source
- Git Push Deploy
- Kubernetes
- Nomad
- K3s
- CLI
- Plugins
---
