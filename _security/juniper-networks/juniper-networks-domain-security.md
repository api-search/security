---
api_specs:
- filename: juniper-networks-apstra-openapi.yml
  format: yaml
  label: Juniper Apstra API
  slug: juniper-apstra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-apstra-openapi.yml
- filename: juniper-networks-junos-telemetry-asyncapi.yml
  format: yaml
  label: Junos XML API
  slug: junos-xml-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/asyncapi/juniper-networks-junos-telemetry-asyncapi.yml
- filename: juniper-networks-mist-openapi.yml
  format: yaml
  label: Juniper Mist API
  slug: juniper-mist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-mist-openapi.yml
- filename: juniper-networks-contrail-openapi.yml
  format: yaml
  label: Juniper Contrail API
  slug: juniper-contrail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-contrail-openapi.yml
- filename: juniper-networks-junos-space-openapi.yml
  format: yaml
  label: Junos Space REST API
  slug: junos-space-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-junos-space-openapi.yml
- filename: juniper-networks-vsrx-openapi.yml
  format: yaml
  label: Juniper vSRX REST API
  slug: juniper-vsrx-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-vsrx-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "digicert.com"
  - 128 issue "letsencrypt.org"
  - 128 issue "sectigo.com"
  - 128 issue "amazon.com"
  - 128 issue "ZScaler.com"
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
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.juniper.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.mist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api.eu.mist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juniper Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juniper Networks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Juniper Networks
provider_slug: juniper-networks
slug: juniper-networks-domain-security
source_filename: juniper-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.juniper.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: api.eu.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: juniper.net\n  dnssec: false\n  caa:\n  - 128 issue \"digicert.com\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"ZScaler.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mist.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:certs@mistsys.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/security/juniper-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Cloud
- Data Center
- Enterprise
- Networking
- SDN
- Security
- Fortune 1000
---
