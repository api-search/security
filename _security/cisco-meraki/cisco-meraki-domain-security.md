---
api_specs:
- filename: cisco-meraki-administered-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Administered
  slug: administered
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-administered-api-openapi.json
- filename: cisco-meraki-appliance-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Appliance
  slug: appliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-appliance-api-openapi.json
- filename: cisco-meraki-camera-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Camera
  slug: camera
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-camera-api-openapi.json
- filename: cisco-meraki-campusgateway-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — campusGateway
  slug: campusgateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-campusgateway-api-openapi.json
- filename: cisco-meraki-cellulargateway-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — cellularGateway
  slug: cellulargateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-cellulargateway-api-openapi.json
- filename: cisco-meraki-devices-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Devices
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-devices-api-openapi.json
- filename: cisco-meraki-insight-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Insight
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-insight-api-openapi.json
- filename: cisco-meraki-licensing-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Licensing
  slug: licensing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-licensing-api-openapi.json
- filename: cisco-meraki-networks-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Networks
  slug: networks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-networks-api-openapi.json
- filename: cisco-meraki-organizations-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Organizations
  slug: organizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-organizations-api-openapi.json
- filename: cisco-meraki-sensor-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Sensor
  slug: sensor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-sensor-api-openapi.json
- filename: cisco-meraki-sm-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Sm
  slug: sm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-sm-api-openapi.json
- filename: cisco-meraki-spaces-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Spaces
  slug: spaces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-spaces-api-openapi.json
- filename: cisco-meraki-switch-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Switch
  slug: switch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-switch-api-openapi.json
- filename: cisco-meraki-wireless-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Wireless
  slug: wireless
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-wireless-api-openapi.json
- filename: cisco-meraki-wirelesscontroller-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — wirelessController
  slug: wirelesscontroller
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-wirelesscontroller-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 128 issuewild "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "identrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meraki.com
  spf: true
hosts:
- cert_expires: Oct 25 15:22:45 2026 GMT
  host: meraki.cisco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:59:42 2026 GMT
  host: api.meraki.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Meraki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Meraki, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Meraki
provider_slug: cisco-meraki
slug: cisco-meraki-domain-security
source_filename: cisco-meraki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meraki.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 15:22:45 2026 GMT\n  hsts: false\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.meraki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 128 issuewild \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: meraki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/security/cisco-meraki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Networking
- Wireless
- Switching
- Security Appliances
- Cloud-Managed Networking
- MDM
- Cameras
- IoT
---
