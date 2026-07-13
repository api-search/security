---
api_specs:
- filename: a10-networks-axapi-openapi.yml
  format: yaml
  label: A10 Networks ACOS aXAPI v3
  slug: a10-networks-axapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a10-networks/refs/heads/main/openapi/a10-networks-axapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: a10networks.com
  spf: true
hosts:
- cert_expires: Oct  9 00:35:26 2026 GMT
  host: www.a10networks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 05:29:58 2026 GMT
  host: documentation.a10networks.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: A10 Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A10 Networks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: A10 Networks
provider_slug: a10-networks
slug: a10-networks-domain-security
source_filename: a10-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.a10networks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:35:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documentation.a10networks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: a10networks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a10-networks/refs/heads/main/security/a10-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Delivery
- Load Balancing
- DDoS Protection
- Application Delivery Controller
- Network Security
- Web Application Firewall
- SSL Decryption
- CGNAT
- Cybersecurity
- Infrastructure
- Kubernetes
- Terraform
- Ansible
- REST API
- Networking
---
