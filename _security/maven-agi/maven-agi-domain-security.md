---
api_specs:
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Conversation API
  slug: maven-agi-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Knowledge API
  slug: maven-agi-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Actions API
  slug: maven-agi-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Users API
  slug: maven-agi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Agents API
  slug: maven-agi-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Events API
  slug: maven-agi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Triggers API
  slug: maven-agi-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI App Settings API
  slug: maven-agi-app-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Analytics API
  slug: maven-agi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mavenagi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mavenagi-apis.com
  spf: false
hosts:
- cert_expires: Sep 16 07:46:09 2026 GMT
  host: www.mavenagi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 17:34:24 2026 GMT
  host: docs.mavenagi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 18:59:34 2026 GMT
  host: www.mavenagi-apis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maven Agi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maven AGI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Maven AGI
provider_slug: maven-agi
slug: maven-agi-domain-security
source_filename: maven-agi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mavenagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:46:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mavenagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:34:24 2026 GMT\n  hsts: null\n- host: www.mavenagi-apis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 18:59:34 2026 GMT\n  hsts: null\ndomains:\n- domain: mavenagi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mavenagi-apis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/security/maven-agi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Agents
- Customer Support
- Customer Experience
- Conversational AI
- Knowledge
---
