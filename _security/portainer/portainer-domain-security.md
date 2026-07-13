---
api_specs:
- filename: portainer-openapi.yml
  format: yaml
  label: Portainer
  slug: portainer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portainer/refs/heads/main/openapi/portainer-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issuewild "usertrust.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: portainer.io
  spf: true
hosts:
- cert_expires: Aug 13 12:21:46 2026 GMT
  host: www.portainer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 02:59:53 2026 GMT
  host: api-docs.portainer.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portainer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portainer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Portainer
provider_slug: portainer
slug: portainer-domain-security
source_filename: portainer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.portainer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 12:21:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.portainer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:59:53 2026 GMT\n  hsts: false\ndomains:\n- domain: portainer.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"usertrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portainer/refs/heads/main/security/portainer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Container Management
- Containers
- Docker
- Kubernetes
---
