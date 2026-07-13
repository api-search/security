---
api_specs:
- filename: thingspeak-channels-api-openapi.yml
  format: yaml
  label: ThingSpeak Channels API
  slug: thingspeak-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-channels-api-openapi.yml
- filename: thingspeak-feeds-api-openapi.yml
  format: yaml
  label: ThingSpeak Feeds API
  slug: thingspeak-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-feeds-api-openapi.yml
- filename: thingspeak-update-api-openapi.yml
  format: yaml
  label: ThingSpeak Update API
  slug: thingspeak-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-update-api-openapi.yml
- filename: thingspeak-mqtt-asyncapi.yml
  format: yaml
  label: ThingSpeak MQTT API
  slug: thingspeak-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/asyncapi/thingspeak-mqtt-asyncapi.yml
- filename: thingspeak-talkback-api-openapi.yml
  format: yaml
  label: ThingSpeak TalkBack API
  slug: thingspeak-talkback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-talkback-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mathworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thingspeak.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: thingspeak.mathworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.mathworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 23:59:59 2026 GMT
  host: api.thingspeak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thingspeak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThingSpeak, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThingSpeak
provider_slug: thingspeak
slug: thingspeak-domain-security
source_filename: thingspeak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thingspeak.mathworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.mathworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: api.thingspeak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mathworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thingspeak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/security/thingspeak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Internet of Things
- Analytics
- Time Series
- MQTT
- MATLAB
- Sensors
- Telemetry
---
