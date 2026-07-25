---
api_specs:
- filename: adobe-launch-builds-api-openapi.yml
  format: yaml
  label: Adobe Launch Builds API
  slug: adobe-launch-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-builds-api-openapi.yml
- filename: adobe-launch-callbacks-api-openapi.yml
  format: yaml
  label: Adobe Launch Callbacks API
  slug: adobe-launch-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-callbacks-api-openapi.yml
- filename: adobe-launch-companies-api-openapi.yml
  format: yaml
  label: Adobe Launch Companies API
  slug: adobe-launch-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-companies-api-openapi.yml
- filename: adobe-launch-data-elements-api-openapi.yml
  format: yaml
  label: Adobe Launch Data Elements API
  slug: adobe-launch-data-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-data-elements-api-openapi.yml
- filename: adobe-launch-edge-network-api-api-openapi.yml
  format: yaml
  label: Adobe Launch Edge Network API API
  slug: adobe-launch-edge-network-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-edge-network-api-api-openapi.yml
- filename: adobe-launch-environments-api-openapi.yml
  format: yaml
  label: Adobe Launch Environments API
  slug: adobe-launch-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-environments-api-openapi.yml
- filename: adobe-launch-extension-packages-api-openapi.yml
  format: yaml
  label: Adobe Launch Extension Packages API
  slug: adobe-launch-extension-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-extension-packages-api-openapi.yml
- filename: adobe-launch-extensions-api-openapi.yml
  format: yaml
  label: Adobe Launch Extensions API
  slug: adobe-launch-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-extensions-api-openapi.yml
- filename: adobe-launch-hosts-api-openapi.yml
  format: yaml
  label: Adobe Launch Hosts API
  slug: adobe-launch-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-hosts-api-openapi.yml
- filename: adobe-launch-libraries-api-openapi.yml
  format: yaml
  label: Adobe Launch Libraries API
  slug: adobe-launch-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-libraries-api-openapi.yml
- filename: adobe-launch-media-edge-api-api-openapi.yml
  format: yaml
  label: Adobe Launch Media Edge API API
  slug: adobe-launch-media-edge-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-media-edge-api-api-openapi.yml
- filename: adobe-launch-properties-api-openapi.yml
  format: yaml
  label: Adobe Launch Properties API
  slug: adobe-launch-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-properties-api-openapi.yml
- filename: adobe-launch-rule-components-api-openapi.yml
  format: yaml
  label: Adobe Launch Rule Components API
  slug: adobe-launch-rule-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-rule-components-api-openapi.yml
- filename: adobe-launch-rules-api-openapi.yml
  format: yaml
  label: Adobe Launch Rules API
  slug: adobe-launch-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-rules-api-openapi.yml
- filename: adobe-launch-search-api-openapi.yml
  format: yaml
  label: Adobe Launch Search API
  slug: adobe-launch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-search-api-openapi.yml
- filename: adobe-launch-secrets-api-openapi.yml
  format: yaml
  label: Adobe Launch Secrets API
  slug: adobe-launch-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-secrets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.io
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: experienceleague.adobe.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: reactor.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Launch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Launch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Launch
provider_slug: adobe-launch
slug: adobe-launch-domain-security
source_filename: adobe-launch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: experienceleague.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: reactor.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/security/adobe-launch-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
---
