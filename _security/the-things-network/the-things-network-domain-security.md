---
api_specs:
- filename: the-things-stack-identity-server-openapi.yml
  format: yaml
  label: The Things Stack Identity Server
  slug: the-things-stack-identity-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-identity-server-openapi.yml
- filename: the-things-stack-application-server-openapi.yml
  format: yaml
  label: The Things Stack Application Server
  slug: the-things-stack-application-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-application-server-openapi.yml
- filename: the-things-stack-network-server-openapi.yml
  format: yaml
  label: The Things Stack Network Server
  slug: the-things-stack-network-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-network-server-openapi.yml
- filename: the-things-stack-gateway-server-openapi.yml
  format: yaml
  label: The Things Stack Gateway Server
  slug: the-things-stack-gateway-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-gateway-server-openapi.yml
- filename: the-things-stack-join-server-openapi.yml
  format: yaml
  label: The Things Stack Join Server
  slug: the-things-stack-join-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-join-server-openapi.yml
- filename: the-things-stack-end-device-registry-openapi.yml
  format: yaml
  label: The Things Stack End Device Registry
  slug: the-things-stack-end-device-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-end-device-registry-openapi.yml
- filename: the-things-stack-integrations-openapi.yml
  format: yaml
  label: The Things Stack Integrations
  slug: the-things-stack-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-integrations-openapi.yml
- filename: the-things-stack-packet-broker-agent-openapi.yml
  format: yaml
  label: The Things Stack Packet Broker Agent
  slug: the-things-stack-packet-broker-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-packet-broker-agent-openapi.yml
- filename: the-things-stack-events-openapi.yml
  format: yaml
  label: The Things Stack Events
  slug: the-things-stack-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-events-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thethingsnetwork.org
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thethingsindustries.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.thethingsnetwork.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.thethingsindustries.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 08:57:00 2026 GMT
  host: console.cloud.thethings.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Things Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Things Network / The Things Stack, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: The Things Network / The Things Stack
provider_slug: the-things-network
slug: the-things-network-domain-security
source_filename: the-things-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thethingsnetwork.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.thethingsindustries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.cloud.thethings.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:57:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thethingsnetwork.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thethingsindustries.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\
  \n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/security/the-things-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LoRaWAN
- IoT
- Internet Of Things
- Open Source
- Network Server
- LPWAN
- Telemetry
- Sensors
- Gateways
- Connectivity
- Apache 2.0
---
