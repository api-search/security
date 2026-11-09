---
api_specs:
- filename: microsoft-skype-deliveryreports-api-openapi.yml
  format: yaml
  label: Microsoft Skype Delivery Reports API
  slug: microsoft-skype-deliveryreports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-deliveryreports-api-openapi.yml
- filename: microsoft-skype-messages-api-openapi.yml
  format: yaml
  label: Microsoft Skype Messages API
  slug: microsoft-skype-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-messages-api-openapi.yml
- filename: microsoft-skype-optoutsadd-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Add API
  slug: microsoft-skype-optoutsadd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsadd-api-openapi.yml
- filename: microsoft-skype-optoutscheck-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Check API
  slug: microsoft-skype-optoutscheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutscheck-api-openapi.yml
- filename: microsoft-skype-optoutsremove-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Remove API
  slug: microsoft-skype-optoutsremove-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsremove-api-openapi.yml
- filename: microsoft-skype-participants-api-openapi.yml
  format: yaml
  label: Microsoft Skype Participants API
  slug: microsoft-skype-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-participants-api-openapi.yml
- filename: microsoft-skype-sms-api-openapi.yml
  format: yaml
  label: Microsoft Skype Sms API
  slug: microsoft-skype-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-sms-api-openapi.yml
- filename: microsoft-skype-threads-api-openapi.yml
  format: yaml
  label: Microsoft Skype Threads API
  slug: microsoft-skype-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-threads-api-openapi.yml
- filename: microsoft-skype-typingnotifications-api-openapi.yml
  format: yaml
  label: Microsoft Skype Typing Notifications API
  slug: microsoft-skype-typingnotifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-typingnotifications-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 issue "microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skype.com
  spf: true
hosts:
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 14:53:05 2027 GMT
  host: www.skype.com
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
name: Microsoft Skype Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Skype, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Skype
provider_slug: microsoft-skype
slug: microsoft-skype-domain-security
source_filename: microsoft-skype-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.skype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 14:53:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: skype.com\n  dnssec: false\n  caa:\n  - 0 issue \"microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-skype/security/microsoft-skype-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- Messaging
- Microsoft
- Video
- Voice
---
