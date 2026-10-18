---
api_specs:
- filename: leaseweb-abuse-api-openapi.yml
  format: yaml
  label: Leaseweb Abuse API
  slug: leaseweb-abuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-abuse-api-openapi.yml
- filename: leaseweb-aggregationpack-api-openapi.yml
  format: yaml
  label: Leaseweb Aggregationpack API
  slug: leaseweb-aggregationpack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-aggregationpack-api-openapi.yml
- filename: leaseweb-dedicatedserver-api-openapi.yml
  format: yaml
  label: Leaseweb Dedicatedserver API
  slug: leaseweb-dedicatedserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-dedicatedserver-api-openapi.yml
- filename: leaseweb-dns-api-openapi.yml
  format: yaml
  label: Leaseweb Dns API
  slug: leaseweb-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-dns-api-openapi.yml
- filename: leaseweb-invoice-api-openapi.yml
  format: yaml
  label: Leaseweb Invoice API
  slug: leaseweb-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-invoice-api-openapi.yml
- filename: leaseweb-ipmgmt-api-openapi.yml
  format: yaml
  label: Leaseweb Ipmgmt API
  slug: leaseweb-ipmgmt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-ipmgmt-api-openapi.yml
- filename: leaseweb-networkequipment-api-openapi.yml
  format: yaml
  label: Leaseweb Networkequipment API
  slug: leaseweb-networkequipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-networkequipment-api-openapi.yml
- filename: leaseweb-objectstorage-api-openapi.yml
  format: yaml
  label: Leaseweb Objectstorage API
  slug: leaseweb-objectstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-objectstorage-api-openapi.yml
- filename: leaseweb-ordering-api-openapi.yml
  format: yaml
  label: Leaseweb Ordering API
  slug: leaseweb-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-ordering-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issue "usertrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: leaseweb.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.leaseweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Leaseweb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leaseweb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Leaseweb
provider_slug: leaseweb
slug: leaseweb-domain-security
source_filename: leaseweb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leaseweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: leaseweb.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"usertrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/security/leaseweb-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cloud
- Infrastructure-as-a-Service
- Bare Metal
- Dedicated Servers
- Object Storage
- DNS
- Hosting
---
