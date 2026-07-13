---
api_specs:
- filename: podman-openapi.yml
  format: yaml
  label: Podman REST API
  slug: podman-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: podman.io
  spf: true
hosts:
- cert_expires: Sep 19 22:09:50 2026 GMT
  host: podman.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:59:03 2026 GMT
  host: docs.podman.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podman, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Podman
provider_slug: podman
slug: podman-domain-security
source_filename: podman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podman.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:09:50 2026 GMT\n  hsts: false\n- host: docs.podman.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:59:03 2026 GMT\n  hsts: false\ndomains:\n- domain: podman.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/security/podman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Native
- Containers
- DevOps
- OCI
- Open Source
---
