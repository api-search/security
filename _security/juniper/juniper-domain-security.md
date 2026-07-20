---
api_specs:
- filename: api-explorer
  format: yaml
  label: Junos Space API
  slug: junos-space-api
  spec_type: OpenAPI
  url: https://[space-server]/api/space/api-explorer
- filename: juniper-apstra-openapi.yml
  format: yaml
  label: Juniper Apstra API
  slug: juniper-apstra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-apstra-openapi.yml
- filename: juniper-junos-rest-api-openapi.yml
  format: yaml
  label: Junos REST API
  slug: junos-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-junos-rest-api-openapi.yml
- filename: docs
  format: yaml
  label: Juniper Mist API
  slug: juniper-mist-api
  spec_type: OpenAPI
  url: https://api.mist.com/api/v1/docs
- filename: juniper-contrail-openapi.yml
  format: yaml
  label: Contrail Networking API
  slug: contrail-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-contrail-openapi.yml
- filename: juniper-atp-cloud-openapi.yml
  format: yaml
  label: Juniper ATP Cloud API
  slug: juniper-atp-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-atp-cloud-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "amazon.com"
  - 128 issue "ZScaler.com"
  - 128 issue "digicert.com"
  - 128 issue "letsencrypt.org"
  - 128 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: juniper.net
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:certs@mistsys.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mist.com
  spf: true
hosts:
- host: developer.juniper.net
  https: false
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.juniper.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.mist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juniper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juniper Networks, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Juniper Networks
provider_slug: juniper
slug: juniper-domain-security
source_filename: juniper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.juniper.net\n  https: false\n- host: www.juniper.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: juniper.net\n  dnssec: false\n  caa:\n  - 128 issue \"amazon.com\"\n  - 128 issue \"ZScaler.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mist.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:certs@mistsys.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/security/juniper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Automation
- Cloud
- Enterprise
- Networking
- SDN
- Security
- Fortune 1000
---
