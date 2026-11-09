---
api_specs:
- filename: microsoft-azure-communication-services-callautomation-api-openapi.yml
  format: yaml
  label: Azure Communication Services Call Automation API
  slug: microsoft-azure-communication-services-callautomation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-callautomation-api-openapi.yml
- filename: microsoft-azure-communication-services-chat-api-openapi.yml
  format: yaml
  label: Azure Communication Services Chat API
  slug: microsoft-azure-communication-services-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-chat-api-openapi.yml
- filename: microsoft-azure-communication-services-email-api-openapi.yml
  format: yaml
  label: Azure Communication Services Email API
  slug: microsoft-azure-communication-services-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-email-api-openapi.yml
- filename: microsoft-azure-communication-services-identity-api-openapi.yml
  format: yaml
  label: Azure Communication Services Identity API
  slug: microsoft-azure-communication-services-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-identity-api-openapi.yml
- filename: microsoft-azure-communication-services-jobrouter-api-openapi.yml
  format: yaml
  label: Azure Communication Services Job Router API
  slug: microsoft-azure-communication-services-jobrouter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml
- filename: microsoft-azure-communication-services-messages-api-openapi.yml
  format: yaml
  label: Azure Communication Services Advanced Messaging API
  slug: microsoft-azure-communication-services-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-messages-api-openapi.yml
- filename: microsoft-azure-communication-services-phonenumbers-api-openapi.yml
  format: yaml
  label: Azure Communication Services Phone Numbers API
  slug: microsoft-azure-communication-services-phonenumbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml
- filename: microsoft-azure-communication-services-rooms-api-openapi.yml
  format: yaml
  label: Azure Communication Services Rooms API
  slug: microsoft-azure-communication-services-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-rooms-api-openapi.yml
- filename: microsoft-azure-communication-services-siprouting-api-openapi.yml
  format: yaml
  label: Azure Communication Services SIP Routing API
  slug: microsoft-azure-communication-services-siprouting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml
- filename: microsoft-azure-communication-services-sms-api-openapi.yml
  format: yaml
  label: Azure Communication Services SMS API
  slug: microsoft-azure-communication-services-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-sms-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Communication Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Communication Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure Communication Services
provider_slug: microsoft-azure-communication-services
slug: microsoft-azure-communication-services-domain-security
source_filename: microsoft-azure-communication-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-communication-services/security/microsoft-azure-communication-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microsoft Azure
- CPaaS
- Calling
- Chat
- Communications
- Contact Center
- Email
- Identity
- Messaging
- Phone Numbers
- Rooms
- Routing
- SIP
- SMS
- Telephony
- Tokens
- Video
- Voice
- WhatsApp
---
