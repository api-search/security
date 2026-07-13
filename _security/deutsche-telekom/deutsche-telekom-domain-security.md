---
api_specs:
- filename: controlplane-rover-server-openapi.yml
  format: yaml
  label: TARDIS Rover API
  slug: tardis-rover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-rover-server-openapi.yml
- filename: controlplane-cpapi-openapi.yml
  format: yaml
  label: TARDIS Controlplane API
  slug: tardis-controlplane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-cpapi-openapi.yml
- filename: controlplane-identity-openapi.yml
  format: yaml
  label: TARDIS Identity API
  slug: tardis-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-identity-openapi.yml
- filename: controlplane-discovery-application-openapi.yml
  format: yaml
  label: TARDIS Discovery Application API
  slug: tardis-discovery-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-discovery-application-openapi.yml
- filename: controlplane-discovery-event-openapi.yml
  format: yaml
  label: TARDIS Discovery Event API
  slug: tardis-discovery-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-discovery-event-openapi.yml
- filename: controlplane-discovery-stargate-openapi.yml
  format: yaml
  label: TARDIS Discovery Stargate API
  slug: tardis-discovery-stargate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-discovery-stargate-openapi.yml
- filename: controlplane-file-manager-openapi.yml
  format: yaml
  label: TARDIS File Manager API
  slug: tardis-file-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-file-manager-openapi.yml
- filename: controlplane-secret-manager-openapi.yml
  format: yaml
  label: TARDIS Secret Manager API
  slug: tardis-secret-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-secret-manager-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telekom.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telekom.de
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.telekom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: developer.telekom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: developer.telekom.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deutsche Telekom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deutsche Telekom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deutsche Telekom
provider_slug: deutsche-telekom
slug: deutsche-telekom-domain-security
source_filename: deutsche-telekom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.telekom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.telekom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: false\n- host: developer.telekom.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: telekom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: telekom.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/security/deutsche-telekom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Telco
- Mobile Network Operator
- CPaaS
- Network API
- 5G
- Cloud
- Identity
- Number Verification
- Open Gateway
- CAMARA
- T-Systems
- T-Mobile
- Magenta
- MagentaBusiness
- API Gateway
- Open Source
- Germany
- Europe
---
