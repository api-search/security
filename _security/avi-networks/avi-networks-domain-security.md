---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avinetworks.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: avinetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Avi Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AVI Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AVI Networks
provider_slug: avi-networks
slug: avi-networks-domain-security
source_filename: avi-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avinetworks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avinetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avi-networks/refs/heads/main/security/avi-networks-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Load Balancing
- Application Delivery
- Networking
- Multi-Cloud
- Web Application Firewall
- Kubernetes Ingress
- Load Balancer
- REST API
---
