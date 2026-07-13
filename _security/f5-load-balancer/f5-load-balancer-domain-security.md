---
api_specs:
- filename: f5-load-balancer-icontrol-rest-openapi.yml
  format: yaml
  label: F5 BIG-IP iControl REST API
  slug: f5-bigip-icontrol-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/openapi/f5-load-balancer-icontrol-rest-openapi.yml
- filename: f5-load-balancer-as3-openapi.yml
  format: yaml
  label: F5 BIG-IP AS3 API
  slug: f5-bigip-as3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/openapi/f5-load-balancer-as3-openapi.yml
- filename: f5-load-balancer-declarative-onboarding-openapi.yml
  format: yaml
  label: F5 BIG-IP Declarative Onboarding API
  slug: f5-bigip-declarative-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/openapi/f5-load-balancer-declarative-onboarding-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:dnsadmin@f5.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: f5.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: clouddocs.f5.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.f5.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: F5 Load Balancer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for F5 Load Balancer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: F5 Load Balancer
provider_slug: f5-load-balancer
slug: f5-load-balancer-domain-security
source_filename: f5-load-balancer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clouddocs.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: www.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: f5.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dnsadmin@f5.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/security/f5-load-balancer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Delivery
- BIG-IP
- Load Balancer
- Networking
- Traffic Management
---
