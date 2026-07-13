---
api_specs:
- filename: mist-ai-openapi.yml
  format: yaml
  label: Juniper Mist Cloud API
  slug: juniper-mist-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mist-ai/refs/heads/main/openapi/mist-ai-openapi.yml
description: ''
domains:
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
- caa:
  - 128 issue "ZScaler.com"
  - 128 issue "digicert.com"
  - 128 issue "letsencrypt.org"
  - 128 issue "sectigo.com"
  - 128 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: juniper.net
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.mist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Mist Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juniper Mist AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Juniper Mist AI
provider_slug: mist-ai
slug: mist-ai-domain-security
source_filename: mist-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.juniper.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mist.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:certs@mistsys.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: juniper.net\n  dnssec: false\n  caa:\n  - 128 issue \"ZScaler.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"amazon.com\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mist-ai/refs/heads/main/security/mist-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- AIOps
- Artificial Intelligence
- Networking
- Wi-Fi
- Wireless LAN
- WAN
- SD-WAN
- Wired
- LAN
- Access Points
- Switches
- Routers
- Marvis
- NAC
- Access Assurance
- Location Services
- Bluetooth LE
- Indoor Location
- Cloud Networking
- Microservices
- Enterprise Networking
- AI Native Networking
---
