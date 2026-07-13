---
api_specs:
- filename: adobe-experience-manager-openapi.yml
  format: yaml
  label: Adobe Experience Manager APIs
  slug: apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-manager/refs/heads/main/openapi/adobe-experience-manager-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobeaemcloud.com
  spf: false
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: business.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- host: author-<tenant>.adobeaemcloud.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''author-<ten'
kind: domain-security
layout: security
method: probed
name: Adobe Experience Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Experience Manager, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Experience Manager
provider_slug: adobe-experience-manager
slug: adobe-experience-manager-domain-security
source_filename: adobe-experience-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: author-<tenant>.adobeaemcloud.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''author-<ten'\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobeaemcloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-manager/refs/heads/main/security/adobe-experience-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Management
- Enterprise CMS
- Digital Asset Management
- Headless CMS
- Content Fragments
- Adaptive Forms
---
