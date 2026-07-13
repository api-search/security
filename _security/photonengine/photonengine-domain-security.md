---
api_specs:
- filename: photonengine-asyncapi.yml
  format: yaml
  label: Photon Realtime Transport Protocol
  slug: photonengine-realtime-transport-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/asyncapi/photonengine-asyncapi.yml
- filename: photonengine-openapi.yml
  format: yaml
  label: Photon Room Lifecycle WebHooks
  slug: photonengine-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/openapi/photonengine-openapi.yml
- filename: photonengine-openapi.yml
  format: yaml
  label: Photon Custom Authentication Webservice Contract
  slug: photonengine-custom-authentication-webservice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/openapi/photonengine-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: photonengine.com
  spf: true
- caa:
  - 0 iodef "mailto:admin@exitgames.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exitgames.com
  spf: true
hosts:
- cert_expires: Aug 19 07:36:22 2026 GMT
  host: www.photonengine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 07:36:22 2026 GMT
  host: doc.photonengine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: ns.exitgames.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Photonengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photon Engine, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Photon Engine
provider_slug: photonengine
slug: photonengine-domain-security
source_filename: photonengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.photonengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:36:22 2026 GMT\n  hsts: false\n- host: doc.photonengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:36:22 2026 GMT\n  hsts: false\n- host: ns.exitgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: photonengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: exitgames.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:admin@exitgames.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/security/photonengine-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gaming
- Multiplayer
- Realtime
- Netcode
- Game Networking
- WebSocket
- Binary Protocol
---
