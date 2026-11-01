---
api_specs:
- filename: cisco-hardware-devices-api-openapi.yml
  format: yaml
  label: Cisco Hardware Devices API
  slug: cisco-hardware-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-devices-api-openapi.yml
- filename: cisco-hardware-administered-api-openapi.yml
  format: yaml
  label: Cisco Hardware Administered API
  slug: cisco-hardware-administered-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-administered-api-openapi.yml
- filename: cisco-hardware-appliance-api-openapi.yml
  format: yaml
  label: Cisco Hardware Appliance API
  slug: cisco-hardware-appliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-appliance-api-openapi.yml
- filename: cisco-hardware-camera-api-openapi.yml
  format: yaml
  label: Cisco Hardware Camera API
  slug: cisco-hardware-camera-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-camera-api-openapi.yml
- filename: cisco-hardware-campusgateway-api-openapi.yml
  format: yaml
  label: Cisco Hardware Campus Gateway API
  slug: cisco-hardware-campusgateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-campusgateway-api-openapi.yml
- filename: cisco-hardware-cellulargateway-api-openapi.yml
  format: yaml
  label: Cisco Hardware Cellular Gateway API
  slug: cisco-hardware-cellulargateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-cellulargateway-api-openapi.yml
- filename: cisco-hardware-insight-api-openapi.yml
  format: yaml
  label: Cisco Hardware Insight API
  slug: cisco-hardware-insight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-insight-api-openapi.yml
- filename: cisco-hardware-licensing-api-openapi.yml
  format: yaml
  label: Cisco Hardware Licensing API
  slug: cisco-hardware-licensing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-licensing-api-openapi.yml
- filename: cisco-hardware-networks-api-openapi.yml
  format: yaml
  label: Cisco Hardware Networks API
  slug: cisco-hardware-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-networks-api-openapi.yml
- filename: cisco-hardware-organizations-api-openapi.yml
  format: yaml
  label: Cisco Hardware Organizations API
  slug: cisco-hardware-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-organizations-api-openapi.yml
- filename: cisco-hardware-sensor-api-openapi.yml
  format: yaml
  label: Cisco Hardware Sensor API
  slug: cisco-hardware-sensor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-sensor-api-openapi.yml
- filename: cisco-hardware-sm-api-openapi.yml
  format: yaml
  label: Cisco Hardware Sm API
  slug: cisco-hardware-sm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-sm-api-openapi.yml
- filename: cisco-hardware-spaces-api-openapi.yml
  format: yaml
  label: Cisco Hardware Spaces API
  slug: cisco-hardware-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-spaces-api-openapi.yml
- filename: cisco-hardware-switch-api-openapi.yml
  format: yaml
  label: Cisco Hardware Switch API
  slug: cisco-hardware-switch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-switch-api-openapi.yml
- filename: cisco-hardware-wireless-api-openapi.yml
  format: yaml
  label: Cisco Hardware Wireless API
  slug: cisco-hardware-wireless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-wireless-api-openapi.yml
- filename: cisco-hardware-wirelesscontroller-api-openapi.yml
  format: yaml
  label: Cisco Hardware Wireless Controller API
  slug: cisco-hardware-wirelesscontroller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-wirelesscontroller-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "digicert.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 128 issuewild "identrust.com"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "globalsign.com"
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
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: intersight.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cisco Hardware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Hardware, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Hardware
provider_slug: cisco-hardware
slug: cisco-hardware-domain-security
source_filename: cisco-hardware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.meraki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: intersight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"digicert.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 128 issuewild \"identrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: meraki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cisco-hardware/security/cisco-hardware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hardware
- Infrastructure
- Networking
- Router
- Switches
---
