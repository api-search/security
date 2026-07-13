---
api_specs:
- filename: bigip-icontrol-rest.yml
  format: yaml
  label: F5 BIG-IP iControl REST API
  slug: f5-big-ip-icontrol-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/openapi/bigip-icontrol-rest.yml
- filename: swagger
  format: yaml
  label: F5 Distributed Cloud API
  slug: f5-distributed-cloud-api
  spec_type: OpenAPI
  url: https://docs.cloud.f5.com/docs/api/swagger
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: f5.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nginx.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.f5.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: docs.cloud.f5.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: docs.nginx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: F5 Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for F5 Networks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: F5 Networks
provider_slug: f5-networks
slug: f5-networks-domain-security
source_filename: f5-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cloud.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\n- host: docs.nginx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: f5.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nginx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/security/f5-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Gateway
- Application Delivery
- Automation
- Edge Computing
- Kubernetes
- Load Balancing
- Multi-Cloud
- NGINX
- Security
- WAF
---
