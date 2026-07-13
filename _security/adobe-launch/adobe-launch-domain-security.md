---
api_specs:
- filename: reactor-api.yml
  format: yaml
  label: Adobe Launch Reactor API
  slug: adobe-launch-reactor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/reactor-api.yml
- filename: extension-api.yml
  format: yaml
  label: Adobe Launch Extension API
  slug: adobe-launch-extension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/extension-api.yml
- filename: event-forwarding-api.yml
  format: yaml
  label: Adobe Experience Platform Event Forwarding API
  slug: adobe-experience-platform-event-forwarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/event-forwarding-api.yml
- filename: data-collection-api.yml
  format: yaml
  label: Adobe Experience Platform Data Collection API
  slug: adobe-experience-platform-data-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/data-collection-api.yml
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
