---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jfrog.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: jfrog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jfrog Container Registry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JFrog Container Registry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JFrog Container Registry
provider_slug: jfrog-container-registry
slug: jfrog-container-registry-domain-security
source_filename: jfrog-container-registry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jfrog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jfrog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jfrog-container-registry/refs/heads/main/security/jfrog-container-registry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Container Images
- Containers
- Docker
- Helm
- JFrog
- Registry
---
