---
api_specs:
- filename: cisco-catalyst-sdwan-administration-and-settings-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Administration and Settings
  slug: administration-and-settings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-administration-and-settings-openapi.json
- filename: cisco-catalyst-sdwan-ux-1-0-configuration-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — UX 1.0 Configuration
  slug: ux-1-0-configuration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-ux-1-0-configuration-openapi.json
- filename: cisco-catalyst-sdwan-ux-2-0-configuration-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — UX 2.0 Configuration
  slug: ux-2-0-configuration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-ux-2-0-configuration-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-wan-system-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-WAN System
  slug: feature-profiles-sd-wan-system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-wan-system-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-wan-transport-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-WAN Transport
  slug: feature-profiles-sd-wan-transport
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-wan-transport-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-wan-service-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-WAN Service
  slug: feature-profiles-sd-wan-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-wan-service-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-others-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - Others
  slug: feature-profiles-others
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-others-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-routing-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-Routing
  slug: feature-profiles-sd-routing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-routing-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-mobility-and-nfv-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - Mobility and NFV
  slug: feature-profiles-mobility-and-nfv
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-mobility-and-nfv-openapi.json
- filename: cisco-catalyst-sdwan-monitoring-and-troubleshooting-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Monitoring and Troubleshooting
  slug: monitoring-and-troubleshooting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-monitoring-and-troubleshooting-openapi.json
- filename: cisco-catalyst-sdwan-sd-wan-services-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — SD-WAN Services
  slug: sd-wan-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-sd-wan-services-openapi.json
- filename: cisco-catalyst-sdwan-partner-integrations-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Partner Integrations
  slug: partner-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-partner-integrations-openapi.json
- filename: cisco-catalyst-sdwan-others-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Others
  slug: others
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-others-openapi.json
description: ''
domains:
- caa:
  - 128 issuewild "identrust.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 128 issuewild "ssl.com"
  - 0 issue "ssl.com"
  - 128 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
hosts:
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Catalyst Sdwan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Catalyst SD-WAN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Catalyst SD-WAN
provider_slug: cisco-catalyst-sdwan
slug: cisco-catalyst-sdwan-domain-security
source_filename: cisco-catalyst-sdwan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"identrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"ssl.com\"\n  - 128 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/security/cisco-catalyst-sdwan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SD-WAN
- Networking
- WAN
- Automation
- Policy
- Enterprise
- Network Management
- Infrastructure as Code
- Observability
- Cisco
---
