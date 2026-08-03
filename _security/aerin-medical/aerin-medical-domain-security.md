---
api_specs:
- filename: aerin-medical-site-openapi.yml
  format: yaml
  label: Aerin Medical Site API (WordPress REST)
  slug: aerin-medical-site-api-wordpress-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/openapi/aerin-medical-site-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aerinmedical.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 04:56:49 2026 GMT
  host: aerinmedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aerin Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerin Medical, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aerin Medical
provider_slug: aerin-medical
slug: aerin-medical-domain-security
source_filename: aerin-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: aerinmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:56:49 2026 GMT\n  hsts: false\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: aerinmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nexposures:\n- id: locator-endpoint-overshares\n  surface: GET https://aerinmedical.com/wp-json/em-locator/v1/locations\n  observed: '2026-07-31'\n  severity: informational\n  finding: >-\n    The anonymously readable doctor-locator collection returns more than the public\n    directory data it renders. Every record echoes a `plugin_settings` object containing the\n    site's Google Maps browser API key and empty\
  \ basic-auth credential fields, and a `post`\n    object whose `post_content` is a JSON blob carrying internal CRM fields — a Salesforce\n    record id, an account number and the named sales representative for that account —\n    alongside the public address and product flags. None of this is shown on\n    https://aerinmedical.com/find-ent-doctor/. 1,012 records are reachable without a\n    credential, with `Access-Control-Allow-Origin: *`.\n  recommendation: >-\n    Shape the locator response to the fields the front end actually renders; restrict the\n    Maps key by HTTP referrer; and route this to the existing Coordinated Vulnerability\n    Disclosure Policy contact (security@aerinmedical.com).\n  disclosure_note: >-\n    Recorded as an observation of a publicly reachable endpoint. The key value, account\n    numbers and personnel names are deliberately NOT reproduced anywhere in this repository.\n  reported: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/security/aerin-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- ENT
- Otolaryngology
- Rhinology
- Radiofrequency Ablation
- Nasal Airway Obstruction
- Chronic Rhinitis
- Physician Locator
- Private Company
---
