---
api_specs:
- filename: f5-mgmt-api-openapi.yml
  format: yaml
  label: F5 BIG-IP iControl REST (Mgmt)
  slug: f5-mgmt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-mgmt-api-openapi.yml
- filename: f5-nginx-plus-api-openapi.yml
  format: yaml
  label: NGINX Plus REST API
  slug: f5-nginx-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-nginx-plus-api-openapi.yml
- filename: f5-big-ip-as3-openapi.yml
  format: yaml
  label: F5 BIG-IP AS3 (Application Services 3 Extension)
  slug: f5-big-ip-as3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-big-ip-as3-openapi.yml
- filename: f5-big-ip-fast-openapi.yml
  format: yaml
  label: F5 BIG-IP Application Services Templates (FAST)
  slug: f5-big-ip-fast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-big-ip-fast-openapi.yml
- filename: f5-big-ip-declarative-onboarding-openapi.yml
  format: yaml
  label: F5 BIG-IP Declarative Onboarding
  slug: f5-big-ip-declarative-onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-big-ip-declarative-onboarding-openapi.yml
- filename: f5-nginx-plus-api-openapi.yml
  format: yaml
  label: F5 NGINX Plus API
  slug: f5-nginx-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-nginx-plus-api-openapi.yml
- filename: f5-nodes-api-openapi.yml
  format: yaml
  label: F5 Networks Nodes API
  slug: f5-networks-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-nodes-api-openapi.yml
- filename: f5-pool-members-api-openapi.yml
  format: yaml
  label: F5 Networks Pool Members API
  slug: f5-networks-pool-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-pool-members-api-openapi.yml
- filename: f5-pools-api-openapi.yml
  format: yaml
  label: F5 Networks Pools API
  slug: f5-networks-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-pools-api-openapi.yml
- filename: f5-profiles-api-openapi.yml
  format: yaml
  label: F5 Networks Profiles API
  slug: f5-networks-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-profiles-api-openapi.yml
- filename: f5-virtual-servers-api-openapi.yml
  format: yaml
  label: F5 Networks Virtual Servers API
  slug: f5-networks-virtual-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-virtual-servers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:dnsadmin@f5.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: f5.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
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
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: clouddocs.f5.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: docs.nginx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: F5 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for F5, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: F5
provider_slug: f5
slug: f5-domain-security
source_filename: f5-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: clouddocs.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: docs.nginx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: f5.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:dnsadmin@f5.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nginx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/security/f5-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application
- Security
- Load Balancing
- API Gateway
- WAF
---
